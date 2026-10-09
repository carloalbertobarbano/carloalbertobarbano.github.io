---
permalink: /research/brainpfn/
title: "BrainPFN"
layout: home
---

<div class="home-narrow" markdown="1">

<header class="page-head">
  <p class="crumb"><a href="/research/">Research</a></p>
  <h1>BrainPFN</h1>
  <p>Amortized brain–behaviour prediction via Prior-Data Fitted Networks.</p>
  <p class="byline"><u>C. A. Barbano</u>, D. Wassermann · Preprint, 2026</p>
  <p class="project-links"><a href="https://inria.hal.science/hal-05767107">Paper (HAL)</a></p>
</header>

<img class="project-figure" src="/images/research/brainpfn.svg" alt="BrainPFN overview: real connectomes, sampled mechanisms, meta-training a transformer, prediction on new data">

<section markdown="1">

## Motivation

The standard way to predict behavioural scores from fMRI is kernel ridge regression (KRR) on functional connectivity (FC) matrices. A separate model has to be fit and tuned for every score and every cohort, and accuracy drops sharply when only a few subjects are available. Small samples are the common case: about 90% of OpenNeuro fMRI datasets have fewer than 100 subjects.

## Method

BrainPFN is a Prior-Data Fitted Network: a transformer trained to approximate the posterior predictive over a prior of brain–behaviour mechanisms.

- **Prior.** Synthetic targets are generated as KRR functions of real FC features, with the kernel (linear, RBF, Laplacian), the dual coefficients, and the noise level sampled at random. The noise level sets the task difficulty.
- **Meta-training pool.** ~7.7k resting-state FC matrices from ~4.9k subjects in 300 public OpenNeuro studies, all preprocessed with the same fMRIPrep-based pipeline and parcellated with Schaefer-400. No behavioural labels are used.
- **Training.** About one billion synthetic context/test pairs drawn from this prior.
- **Inference.** A labelled context from a new cohort is passed through the frozen network together with the query subjects. There is no refitting, gradient step, or hyperparameter search per score or cohort.

## Results

Evaluation on four independent cohorts (HCP Young Adult, HCP-Aging, Cam-CAN, AOMIC-ID1000) and 85 behavioural targets, against Ridge/KRR and the foundation models Brain-JEPA, BrainMass, Brain-Semantoks, and TabPFN v2:

- BrainPFN is the only model that consistently beats Ridge with small samples, including on general cognition in every cohort.
- The advantage holds for movie-watching and task fMRI, although BrainPFN was meta-trained on resting-state data only.
- As the number of labelled subjects grows (around N ≈ 200), Ridge catches up on HCP-YA and HCP-Aging.

<figure>
  <img class="project-figure" src="/images/research/brainpfn-results.png" alt="Mean Pearson r against context size N and log-AULC for each model on the four cohorts">
  <figcaption>Mean Pearson r against context size N (top) and area under the learning curve (bottom) on the four evaluation cohorts. * marks results significantly better than Ridge (p &lt; 0.05).</figcaption>
</figure>

## Release

The meta-training pool, code, and model checkpoints will be made public upon acceptance.

</section>

</div>
