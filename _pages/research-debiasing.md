---
layout: single
title: "Collateral Learning and Debiasing"
permalink: /research/debiasing-collateral-learning/
author_profile: true
---

<div style="overflow: auto;">
  <img src="/images/research/axis2.png" style="float: left; margin-right: 30px; margin-bottom: 20px; max-width: 45%;">
  
  <h2>Collateral Learning and Debiasing</h2>
  
  <p>Bias in training data is ubiquitous in machine learning, particularly in medical and scientific applications. My research addresses both technical solutions and interpretability aspects of learning from biased data.</p>
  
  <h3>Key Research Areas</h3>
  
  <p><strong>Spurious Correlations and Confounders</strong><br>
  Real-world datasets contain numerous spurious correlations that can be exploited by deep learning models. When the actual target variable shares correlations with confounding factors (e.g., age, sex, site effects), models may learn the wrong patterns, leading to poor generalization and unreliable predictions.</p>
  
  <p><strong>Unbiased Learning Methods</strong><br>
  Developing algorithms that can learn the true predictive signals while ignoring spurious correlations is critical. This includes both supervised and unsupervised approaches that disentangle the factors of variation in the data.</p>
  
  <p><strong>Interpretability and Human Understanding</strong><br>
  Rather than just correcting for bias, I focus on methods that provide human-interpretable descriptions of the spurious correlations discovered in the data. This facilitates domain expert validation and understanding of model failures.</p>
  
  <h3>Selected Works</h3>
  
  <ul>
    <li><strong>End: Entangling and Disentangling Deep Representations for Bias Correction</strong> - CVPR, 2021
      <ul>
        <li>Seminal work on learning disentangled representations</li>
        <li>Enables discovery and removal of biased factors</li>
        <li>Improved robustness across domains</li>
      </ul>
    </li>
    <li><strong>Explainable AI for Identifying Spurious Correlations</strong> - arxiv:2408.09570
      <ul>
        <li>Framework for detecting hidden correlations in training data</li>
        <li>Provides interpretable explanations of discovered biases</li>
        <li>Supports clinical validation of AI systems</li>
      </ul>
    </li>
  </ul>
  
  <h3>Applications</h3>
  
  <ul>
    <li><strong>Clinical Robustness</strong>: Ensuring that diagnostic AI systems perform consistently across different hospitals and imaging protocols</li>
    <li><strong>Fairness</strong>: Addressing demographic biases in medical AI to ensure equitable healthcare</li>
    <li><strong>Generalization</strong>: Improving model performance when deployed to new populations with different bias structures</li>
  </ul>
  
  <h3>Future Directions</h3>
  
  <p>Ongoing research explores multi-task and meta-learning approaches to automatically identify and adapt to unknown biases in new domains, creating more robust and trustworthy AI systems for clinical deployment.</p>
</div>
