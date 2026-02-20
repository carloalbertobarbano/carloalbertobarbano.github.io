---
layout: single
title: "Foundation and Normative Modeling in Neuroimaging"
permalink: /research/foundation-normative-modeling/
author_profile: true
---

<div style="overflow: auto;">
  <img src="/images/research/axis3.png" style="float: left; margin-right: 30px; margin-bottom: 20px; max-width: 45%;">
  
  <h2>Foundation and Normative Modeling in Neuroimaging</h2>
  
  <p>Foundation models—large neural networks pre-trained on vast amounts of data—have revolutionized natural language processing and computer vision. My research extends this paradigm to neuroimaging, developing models that learn generalizable brain representations from large-scale datasets.</p>
  
  <h3>Key Research Areas</h3>
  
  <p><strong>Large-Scale Neuroimaging Pre-Training</strong><br>
  The key insight is that brain imaging exhibits consistent anatomical and functional patterns across populations. By pre-training on large, diverse neuroimaging datasets, we can learn robust representations that capture fundamental brain organization principles.</p>
  
  <p><strong>Transfer to Clinical Populations</strong><br>
  Once trained on general populations, these foundation models can be effectively transferred to smaller clinical cohorts with specific conditions (neurodegenerative disorders, psychiatric disorders, brain tumors, etc.), dramatically improving performance with limited labeled data.</p>
  
  <p><strong>Normative Modeling Framework</strong><br>
  Normative models establish what constitutes "normal" variation in brain structure and function across a population. Deviations from these norms can indicate disease or disorder. By learning from large healthy populations, we create better baselines for identifying pathology.</p>
  
  <p><strong>Multimodal Integration</strong><br>
  Brain imaging often involves multiple modalities (structural MRI, functional MRI, diffusion imaging, etc.). Foundation models can leverage relationships between modalities to learn richer representations than any single modality alone.</p>
  
  <h3>Selected Works</h3>
  
  <ul>
    <li><strong>Anatomical Foundation Models for Brain MRIs</strong> - Pattern Recognition Letters, 2025
      <ul>
        <li>Large-scale pre-training on structural MRI data</li>
        <li>Demonstrates superior transfer performance to clinical tasks</li>
        <li>Enables few-shot learning on rare diseases</li>
      </ul>
    </li>
    <li><strong>From General to Specific: Learning Neuroimaging Models That Transfer</strong> - arxiv:2408.07079
      <ul>
        <li>Theoretical and empirical analysis of transfer learning in neuroimaging</li>
        <li>Establishes best practices for foundation model development</li>
        <li>Benchmarks against task-specific training</li>
      </ul>
    </li>
  </ul>
  
  <h3>Clinical Impact</h3>
  
  <ul>
    <li><strong>Rare Disease Diagnosis</strong>: Enable detection of rare neurological conditions with limited training examples</li>
    <li><strong>Population Studies</strong>: Identify subtle population differences in brain organization</li>
    <li><strong>Personalized Medicine</strong>: Create patient-specific deviation scores from normative trends</li>
    <li><strong>Aging Research</strong>: Better characterize healthy aging while detecting early pathological changes</li>
  </ul>
  
  <h3>Research Community</h3>
  
  <p>This work is conducted as part of the <a href="https://team.inria.fr/mind/">MIND (Models and Inference for Neuroimaging Data)</a> team at Inria Saclay, collaborating with leading neuroimaging researchers and clinical partners.</p>
  
  <h3>Future Directions</h3>
  
  <p>Ongoing work aims to develop:</p>
  <ul>
    <li>Multi-modal foundation models integrating structural, functional, and diffusion MRI</li>
    <li>Privacy-preserving federated learning approaches for sensitive clinical data</li>
    <li>Uncertainty quantification for clinical decision support</li>
    <li>Interpretable normative models that explain deviations from population norms</li>
  </ul>
</div>
