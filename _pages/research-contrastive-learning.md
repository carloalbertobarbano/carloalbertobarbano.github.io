---
layout: single
title: "Contrastive Representation Learning"
permalink: /research/contrastive-learning/
author_profile: true
---

<div style="overflow: auto;">
  <img src="/images/research/axis1.png" style="float: left; margin-right: 30px; margin-bottom: 20px; max-width: 45%;">
  
  <h2>Contrastive Representation Learning</h2>
  
  <p>Contrastive learning has become a cornerstone of my research, particularly in the context of medical imaging and neuroimaging. This approach enables models to learn meaningful representations by maximizing the similarity between related samples while minimizing it for unrelated ones.</p>
  
  <h3>Key Research Areas</h3>
  
  <p><strong>Self-Supervised Learning in Medical Imaging</strong><br>
  Learning robust representations from unlabeled medical data is crucial for clinical applications where annotations are expensive and scarce. My work focuses on developing contrastive methods that can effectively capture anatomical and pathological features in brain MRI and other medical imaging modalities.</p>
  
  <p><strong>Unbiased Contrastive Learning</strong><br>
  A significant contribution in this area is the development of unbiased contrastive learning frameworks that mitigate the impact of spurious correlations in training data. This ensures that learned representations generalize better across different datasets and populations.</p>
  
  <p><strong>Multi-Site Harmonization</strong><br>
  Brain imaging studies often involve data from multiple imaging centers with different acquisition protocols. Contrastive learning provides a natural framework for learning representations that are invariant to these site-specific variations while preserving clinically relevant information.</p>
  
  <h3>Selected Works</h3>
  
  <ul>
    <li><strong>Unbiased Supervised Contrastive Learning</strong> - ICLR, 2023
      <ul>
        <li>Theoretical framework for eliminating bias in contrastive objectives</li>
        <li>Demonstrates improved generalization across datasets</li>
      </ul>
    </li>
    <li><strong>Contrastive Learning for Regression in Multi-Site Brain Age Prediction</strong> - ISBI, 2023 (Best Poster Award)
      <ul>
        <li>Applies contrastive learning to predict brain age from MRI</li>
        <li>Shows superior performance in multi-site settings</li>
      </ul>
    </li>
    <li><strong>Integrating Prior Knowledge in Contrastive Learning with Kernel</strong> - ICML, 2023
      <ul>
        <li>Incorporates domain knowledge into contrastive objectives using kernel methods</li>
      </ul>
    </li>
  </ul>
  
  <h3>Future Directions</h3>
  
  <p>Ongoing work aims to extend contrastive learning to foundation models for neuroimaging, where models pre-trained on large-scale datasets can be effectively transferred to smaller clinical cohorts with specific disorders.</p>
</div>
