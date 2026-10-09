---
permalink: /research/anatcl/
title: "AnatCL"
layout: home
---

<div class="home-narrow" markdown="1">

<header class="page-head">
  <p class="crumb"><a href="/research/">Research</a></p>
  <h1>AnatCL</h1>
  <p>Anatomical foundation models for brain MRIs.</p>
  <p class="byline"><u>C. A. Barbano</u>, M. Brunello, B. Dufumier, M. Grangetto · Pattern Recognition Letters, 2025</p>
  <p class="project-links"><a href="https://www.sciencedirect.com/science/article/pii/S0167865525003848">Paper</a><a href="https://github.com/EIDOSLAB/AnatCL">Code and pre-trained models</a></p>
</header>

<img class="project-figure" src="/images/research/anatcl.svg" alt="AnatCL overview: anatomical MRIs, anatomical similarity, contrastive pre-training, linear probing">

<section markdown="1">

## Motivation

Weakly supervised contrastive pre-training on brain MRI usually relies on a single attribute, the subject's age, to decide which scans should be close in representation space. Anatomical measures such as cortical thickness carry more information about the brain, and they can be computed from the MRI itself with standard tools such as FreeSurfer, without extra labels.

## Method

AnatCL extends weakly supervised contrastive learning to multiple attributes.

- **Anatomical similarity.** For two scans, a degree of positiveness is computed from three FreeSurfer measures: cortical thickness, gray matter volume, and surface area, on the Desikan-Killiany (68 regions) or Destrieux (148 regions) atlas.
- **Local and global variants.** The local variant compares the measures region by region; the global variant compares each measure across the whole brain.
- **Objective.** The anatomical loss is combined with an age-based loss (y-Aware): L = λ₁ L<sub>AnatCL</sub> + λ₂ L<sub>age</sub>.
- **Pre-training.** A 3D ResNet-18 trained on the healthy subjects of OpenBHB (3,984 T1-weighted MRIs, VBM preprocessing).

## Results

The pre-trained encoder is frozen and evaluated with linear probing on 12 downstream tasks (ADNI, OASIS-3, SchizConnect, ABIDE I) and 10 clinical assessment scores, against SimCLR, brain-age regression (L1), y-Aware, and ExpW.

- AnatCL gives the best average performance across tasks and the lowest brain-age error on OpenBHB (MAE 2.55 years).
- It leads on most schizophrenia tasks, on Asperger's and PDD-NOS, and on Alzheimer's disease detection on OASIS-3.
- Ablations show that combining anatomical and age information works better than either one alone.

<figure>
  <img class="project-figure figure--narrow" src="/images/research/anatcl-radar.png" alt="Radar plot of balanced accuracy for AnatCL and baselines on the phenotyping tasks">
  <figcaption>Balanced accuracy on the phenotyping tasks for AnatCL (local and global) and the baselines.</figcaption>
</figure>

## Independent evaluation: cross-scanner reliability

An independent study by <a href="https://www.medrxiv.org/content/10.64898/2026.03.23.26348808v2">Navarro-González et al.</a> (medRxiv, 2026) measured how stable brain MRI foundation model embeddings are across scanners, using a travelling-heads dataset (20 participants, 8 scanners, 3 vendors). AnatCL had the highest cross-scanner reliability of the models tested (ICC 0.97), above the FreeSurfer morphometric baseline (0.93), y-Aware (0.81), and purely self-supervised models (0.25–0.45). Its representations are therefore the least affected by scanner and site.

## Code

Code and pre-trained models are available on [GitHub](https://github.com/EIDOSLAB/AnatCL).

</section>

</div>
