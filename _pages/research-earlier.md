---
permalink: /research/earlier-work/
title: "Earlier work"
layout: home
---

<div class="home-narrow" markdown="0">

<header class="page-head">
  <p class="crumb"><a href="/research/">Research</a></p>
  <h1>Earlier work</h1>
  <p>Work from my Ph.D. at Télécom Paris and the University of Turin (2020–2023) and my postdoc in the <a href="https://eidos.di.unito.it/">EIDOS group</a> at the University of Turin (2023–2025), on deep learning for medical imaging and neuroimaging.</p>
</header>

<section class="theme" id="contrastive-learning">
  <div class="theme-text">
    <h2>Contrastive representation learning</h2>
    <p>Contrastive learning trains a model to bring related samples together in representation space and push unrelated ones apart. I worked on contrastive objectives for medical imaging and neuroimaging, where labels are limited and data come from many sites.</p>
    <ul class="theme-items">
      <li><strong>ε-SupInfoNCE.</strong> A generalization of InfoNCE through metric constraints between positive and negative distances.
        <span class="ref"><a href="https://openreview.net/forum?id=Ph5cJSfD2XN">Unbiased Supervised Contrastive Learning</a>, ICLR 2023</span></li>
      <li><strong>Contrastive learning for regression.</strong> Alignment and repulsion weighted by continuous targets instead of binary positives and negatives, applied to multi-site brain age prediction.
        <span class="ref"><a href="https://arxiv.org/abs/2211.08326">Contrastive learning for regression in multi-site brain age prediction</a>, ISBI 2023 (best poster award) · extended in <a href="https://doi.org/10.1016/j.patrec.2026.02.032">Pattern Recognition Letters 2026</a></span></li>
      <li><strong>Prior knowledge with kernels.</strong> Integrating prior information into contrastive learning through kernels.
        <span class="ref"><a href="https://proceedings.mlr.press/v202/dufumier23a.html">Integrating Prior Knowledge in Contrastive Learning with Kernel</a>, ICML 2023</span></li>
    </ul>
  </div>
  <img class="theme-figure" src="/images/research/earlier-1.jpg" alt="ε-SupInfoNCE metric constraints and contrastive learning for regression">
</section>

<section class="theme theme--wide" id="debiasing">
  <div class="theme-text">
    <h2>Collateral learning and debiasing</h2>
    <p>Training data often contain spurious correlations, or biases, that a model can learn instead of the intended task. I worked on methods to learn representations that do not rely on these biases, with and without bias labels.</p>
    <ul class="theme-items">
      <li><strong>EnD.</strong> A regularization that aligns bias-conflicting samples and repels bias-aligned positives.
        <span class="ref"><a href="https://openaccess.thecvf.com/content/CVPR2021/html/Tartaglione_EnD_Entangling_and_Disentangling_Deep_Representations_for_Bias_Correction_CVPR_2021_paper.html">EnD: Entangling and Disentangling deep representations for bias correction</a>, CVPR 2021</span></li>
      <li><strong>FairKL.</strong> Moment matching between the distributions of bias-conflicting and bias-aligned positives.
        <span class="ref"><a href="https://openreview.net/forum?id=Ph5cJSfD2XN">Unbiased Supervised Contrastive Learning</a>, ICLR 2023</span></li>
      <li><strong>Unsupervised debiasing.</strong> Debiasing without bias labels, using bias pseudo-labels from a bias predictor.
        <span class="ref"><a href="https://arxiv.org/abs/2204.12941">Unsupervised Learning of Unbiased Visual Representations</a>, IEEE TAI 2024</span></li>
      <li><strong>Debiasing and privacy.</strong>
        <span class="ref"><a href="https://openaccess.thecvf.com/content/ICCV2021W/RPRMI/html/Barbano_Bridging_the_Gap_Between_Debiasing_and_Privacy_for_Deep_Learning_ICCVW_2021_paper.html">Bridging the gap between debiasing and privacy for deep learning</a>, ICCV Workshops 2021</span></li>
    </ul>
  </div>
  <img class="theme-figure" src="/images/research/earlier-2.jpg" alt="EnD, FairKL and unsupervised debiasing">
</section>

<section class="theme" id="medical-imaging">
  <div class="theme-text">
    <h2>Medical imaging applications</h2>
    <ul class="theme-items">
      <li><strong>COVID-19 from chest X-rays</strong>, from small-data training to clinical validation.
        <span class="ref"><a href="https://doi.org/10.3390/ijerph17186933">IJERPH 2020</a> · <a href="https://doi.org/10.1007/978-3-031-06427-2_15">ICIAP 2022</a> · <a href="https://arxiv.org/abs/2405.11598">ISBI 2024</a> · <a href="https://www.sciencedirect.com/science/article/pii/S2001037024004161">CSBJ 2024</a></span></li>
      <li><strong>Histopathology</strong>: the UniToPatho dataset for colorectal polyp classification, and multi-target stain normalization.
        <span class="ref"><a href="https://ieeexplore.ieee.org/abstract/document/9506198/">ICIP 2021</a> · MOVI 2024</span></li>
      <li><strong>Efficient networks</strong>: Simplify, a Python library for optimizing pruned neural networks.
        <span class="ref"><a href="https://doi.org/10.1016/j.softx.2021.100907">SoftwareX 2022</a></span></li>
    </ul>
  </div>
</section>

</div>
