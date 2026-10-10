---
description: "Research of Carlo Alberto Barbano: foundation models for fMRI (BrainPFN, Open-fMIND, TIMBER) and foundation and normative models of brain anatomy (AnatCL)."
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
  <article class="project project--featured" id="fmri">
    <div class="project-head">
      <h3>Foundation models for fMRI</h3>
    </div>
    <p>Foundation models pretrained on large fMRI collections should transfer to new cohorts and tasks. For predicting individual phenotypes, however, they often do not outperform kernel ridge regression (KRR) on functional connectivity (FC). This line of work studies when and how they can, through open pretraining data, prediction models for small cohorts, and better pretraining targets and objectives.</p>
    <img class="project-figure" src="/images/research/brainpfn.svg" alt="BrainPFN overview">
    <ul class="theme-items">
      <li id="brainpfn"><strong><a href="/research/brainpfn/">BrainPFN</a>.</strong> Amortized brain–behaviour prediction with Prior-Data Fitted Networks. A transformer meta-trained on synthetic regression tasks built from real FC matrices predicts behavioural scores from a labelled context in one forward pass, without refitting.
        <span class="ref"><a href="https://inria.hal.science/hal-05767107">BrainPFN: Amortized Brain-Behaviour Prediction via Prior-Data Fitted Networks</a>, Preprint 2026 · With D. Wassermann · <a href="/research/brainpfn/">Details</a></span></li>
      <li id="open-fmind"><strong><a href="https://pages.saclay.inria.fr/carlo.barbano/open-fmind/">Open-fMIND</a>.</strong> An open-access fMRI timeseries collection for self-supervised training of brain foundation models. It is built entirely from public OpenNeuro studies, uniformly preprocessed with a single pipeline, and released as parcellated ROI timeseries and FC matrices for several atlases. BrainPFN and the spectral filter work below are trained on data from Open-fMIND.
        <ul class="project-stats">
          <li><strong>14,016</strong> subjects</li>
          <li><strong>52,505</strong> functional runs</li>
          <li><strong>52</strong> atlases</li>
          <li><strong>2.73M</strong> ROI timeseries</li>
        </ul>
        <span class="ref">Coming soon · Joint work with G. Marraffini and D. Wassermann · <a href="https://pages.saclay.inria.fr/carlo.barbano/open-fmind/">Project page</a></span></li>
      <li id="connectome-spectrum"><strong>Spectral filtering of FC as a pretraining target.</strong> Kernel ridge regression on FC still predicts individual phenotypes better than the brain foundation models we tested. A spectral filter that recalibrates the eigenvalues of each subject's FC matches or exceeds this baseline across 5 datasets, 11 parcellations and 6 targets. Used as a pretraining target, it lets a small encoder trained on about 4,000 hours of fMRI from 162 open datasets perform on par with the best of 6 published foundation models, with an order of magnitude fewer parameters.
        <span class="ref"><a href="https://arxiv.org/abs/2609.37642">Flattening the Connectome Spectrum: A Spectral Filter for FC Induces a Pretraining Target for fMRI Encoders</a>, Preprint 2026 · G. Marraffini, V. Shevchenko, <u>C. A. Barbano</u>, D. Wassermann</span></li>
      <li id="timber"><strong>TIMBER.</strong> Data-efficient self-supervised representation learning directly from raw fMRI time series, without predefined atlases or connectivity measures. Trained without labels on 200 subjects from the Human Connectome Project, it performs competitively on sex classification and cognitive score prediction, and generalizes to autism detection on ABIDE I.
        <span class="ref"><a href="https://hal.science/hal-05632181">TIMBER: Data-Efficient Self-Supervised Representation Learning for fMRI Time Series</a>, Preprint 2026 · A. Le Bris, <u>C. A. Barbano</u>, D. Wassermann</span></li>
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
        <span class="ref"><a href="https://www.sciencedirect.com/science/article/pii/S0167865525003848">Anatomical foundation models for brain MRIs</a>, Pattern Recognition Letters 2026 · With M. Brunello, B. Dufumier, M. Grangetto · <a href="/research/anatcl/">Details</a></span></li>
      <li><strong>Robust brain age estimation</strong> with contrastive learning. An extension of our ISBI 2023 work to over 20,000 T1 scans from four public datasets, studying generalization to unseen sites, robustness to site effects, and accelerated ageing in cognitive impairment and Alzheimer's disease.
        <span class="ref"><a href="https://doi.org/10.1016/j.patrec.2026.02.032">Robust brain age estimation from structural MRI with contrastive learning</a>, Pattern Recognition Letters 2026 · With B. Dufumier, E. Duchesnay, M. Grangetto, P. Gori</span></li>
      <li><strong>Normative modelling of brain anatomy</strong> for unsupervised anomaly detection, with a conditional diffusion model.
        <span class="ref"><a href="https://www.sciencedirect.com/science/article/pii/S016786552500371X">Unsupervised contrastive analysis for anomaly detection in brain MRIs via conditional diffusion models</a>, Pattern Recognition Letters 2026 · C. Patrício, <u>C. A. Barbano</u>, A. Fiandrotti, R. Renzulli, M. Grangetto, L. F. Teixeira, J. C. Neves</span></li>
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
