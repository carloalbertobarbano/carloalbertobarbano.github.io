---
permalink: /research/
title: "Research"
layout: home
---

<div class="home-narrow" markdown="1">

<header class="page-head">
  <h1>Research</h1>
  <p>Foundation models for fMRI and brain–behaviour prediction in the <a href="https://team.inria.fr/mind/">MIND</a> team at Inria Saclay, and foundation and normative models of brain anatomy.</p>
</header>

<section>
  <article class="project project--featured" id="brainpfn">
    <div class="project-head">
      <h3><a href="/research/brainpfn/">BrainPFN</a></h3>
      <span class="project-tag">Preprint, 2026</span>
    </div>
    <p>Amortized brain–behaviour prediction with Prior-Data Fitted Networks. A transformer meta-trained on synthetic regression tasks built from real FC matrices predicts behavioural scores from a labelled context in one forward pass.</p>
    <img class="project-figure" src="/images/research/brainpfn.svg" alt="BrainPFN overview">
    <p class="project-links"><a href="/research/brainpfn/">Details</a><a href="https://inria.hal.science/hal-05767107">Paper (HAL)</a></p>
  </article>

  <article class="project project--split" id="open-fmind">
      <div class="project-body">
    <div class="project-head">
      <h3>Open-fMIND</h3>
      <span class="project-tag">Coming soon</span>
    </div>
    <p>An open-access fMRI timeseries collection for self-supervised training of brain foundation models. It is built entirely from public OpenNeuro studies, uniformly preprocessed with a single pipeline, and released as parcellated ROI timeseries and FC matrices for several atlases, with dataset-level provenance.</p>
    <p>Joint work with G. Marraffini and D. Wassermann.</p>
    <p class="project-links"><a href="https://pages.saclay.inria.fr/carlo.barbano/open-fmind/">Project page</a></p>
      </div>
    <ul class="project-stats">
      <li><strong>14,016</strong> subjects</li>
      <li><strong>52,505</strong> functional runs</li>
      <li><strong>52</strong> atlases</li>
      <li><strong>2.73M</strong> ROI timeseries</li>
    </ul>
    </article>

  <article class="project" id="brain-anatomy">
    <div class="project-head">
      <h3>Foundation and normative models of brain anatomy</h3>
    </div>
    <p>Pre-training on large anatomical MRI datasets to learn brain representations that transfer to many downstream tasks, and modelling the healthy population to detect and follow deviations from it.</p>
    <img class="project-figure" src="/images/research/anatcl.svg" alt="AnatCL overview: anatomical MRIs, anatomical similarity, contrastive pre-training, linear probing">
    <ul class="theme-items">
      <li><strong><a href="/research/anatcl/">AnatCL</a>.</strong> An open-source foundation model for anatomical brain MRI, trained with contrastive learning guided by anatomical features and age. In an independent travelling-heads benchmark, its representations were the most reliable across scanners among the models tested.
        <span class="ref"><a href="https://www.sciencedirect.com/science/article/pii/S0167865525003848">Anatomical foundation models for brain MRIs</a>, Pattern Recognition Letters 2026 · <a href="/research/anatcl/">Details</a></span></li>
      <li><strong>Robust brain age estimation</strong> with contrastive learning. An extension of our ISBI 2023 work to over 20,000 T1 scans from four public datasets, studying generalization to unseen sites, robustness to site effects, and accelerated ageing in cognitive impairment and Alzheimer's disease.
        <span class="ref"><a href="https://doi.org/10.1016/j.patrec.2026.02.032">Robust brain age estimation from structural MRI with contrastive learning</a>, Pattern Recognition Letters 2026</span></li>
      <li><strong>Normative modelling of brain anatomy</strong> for unsupervised anomaly detection, with a conditional diffusion model.
        <span class="ref"><a href="https://www.sciencedirect.com/science/article/pii/S016786552500371X">Unsupervised contrastive analysis for anomaly detection in brain MRIs via conditional diffusion models</a>, Pattern Recognition Letters 2026</span></li>
      <li><strong>Modelling brain and disease development</strong> from longitudinal and multimodal brain imaging, with brain age prediction and generative models.
        <span class="ref">With Akshita Kumar, Ph.D. student co-supervised with Pietro Gori · <a href="https://theses.fr/s428919">Thesis</a></span></li>
    </ul>
  </article>

  <article class="project" id="earlier">
    <div class="project-head"><h3><a href="/research/earlier-work/">Earlier work</a></h3><span class="project-tag">2020–2025</span></div>
    <p>Contrastive representation learning, debiasing, and medical imaging applications.</p>
    <p class="project-links"><a href="/research/earlier-work/">Details</a><a href="{{ site.author.googlescholar }}">Publications</a></p>
  </article>
</section>

</div>
