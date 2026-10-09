---
permalink: /
title: "Carlo Alberto Barbano"
layout: home
redirect_from: [/about/, /about.html]
---

<header class="home-hero">
  <div class="wrap">
    <img class="hero-photo" src="/images/profile-hero.jpg" alt="Carlo Alberto Barbano">
    <div class="hero-text">
      <h1>Carlo Alberto Barbano</h1>
      <p class="lede">I am a Starting Researcher in the <a href="https://team.inria.fr/mind/">MIND</a> team at Inria Saclay, working on foundation models for fMRI and brain–behaviour prediction.</p>
      <nav class="home-links">
        <a href="mailto:carlo.barbano@inria.fr">Contact</a>
        <a href="{{ site.author.googlescholar }}">Google Scholar</a>
        <a href="https://github.com/{{ site.author.github }}">GitHub</a>
        <a href="{{ site.author.orcid }}">ORCID</a>
      </nav>
    </div>
  </div>
</header>

<section class="home-research">
  <div class="wrap" markdown="0">
    <h2>Research</h2>

    <article class="project project--featured">
      <div class="project-head">
        <h3><a href="/research/brainpfn/">BrainPFN</a></h3>
        <p class="project-sub">Amortized brain–behaviour prediction with Prior-Data Fitted Networks.</p>
        <span class="project-tag">Preprint, 2026</span>
      </div>
      <img class="project-figure" src="/images/research/brainpfn.svg" alt="BrainPFN overview: real connectomes, sampled mechanisms, meta-training a transformer, prediction on new data">
      <p class="project-links"><a href="/research/brainpfn/">Details</a><a href="https://inria.hal.science/hal-05767107">Paper (HAL)</a></p>
    </article>

    <article class="project project--split">
      <div class="project-body">
        <div class="project-head">
          <h3><a href="/research/#open-fmind">Open-fMIND</a></h3>
          <span class="project-tag">Coming soon</span>
        </div>
        <p>An open fMRI collection built from public OpenNeuro studies, uniformly preprocessed and released as parcellated timeseries and FC matrices for several atlases.</p>
        <p class="project-links"><a href="https://pages.saclay.inria.fr/carlo.barbano/open-fmind/">Project page</a></p>
      </div>
      <ul class="project-stats">
        <li><strong>14,016</strong> subjects</li>
        <li><strong>52,505</strong> functional runs</li>
        <li><strong>52</strong> atlases</li>
      </ul>
    </article>

    <article class="project project--media">
      <div class="project-body">
        <div class="project-head">
          <h3><a href="/research/#brain-anatomy">Foundation and normative models of brain anatomy</a></h3>
        </div>
        <p>AnatCL, a foundation model for anatomical brain MRI, normative models for anomaly detection, and models of brain and disease development.</p>
        <p class="project-links"><a href="/research/anatcl/">AnatCL</a><a href="/research/#brain-anatomy">More</a></p>
      </div>
      <img class="project-media" src="/images/research/anatcl-card.svg" alt="AnatCL: anatomical MRI, morphological descriptors and contrastive pre-training">
    </article>

    <p class="home-more"><a href="/research/earlier-work/">Earlier work</a> covered contrastive learning and debiasing. If you are interested in collaborating, <a href="mailto:carlo.barbano@inria.fr">contact me</a>.</p>
  </div>
</section>

<section class="home-updates">
  <div class="wrap home-cols" markdown="0">
    <div class="home-news">
    <h2>News</h2>
    <ul>
      <li><span class="date">Sep. 2026</span><span><a href="https://inria.hal.science/hal-05767107">BrainPFN</a> preprint is out.</span></li>
      <li><span class="date">Nov. 2025</span><span>I am now a <strong>Starting Researcher</strong> at <a href="https://team.inria.fr/mind/">Inria Saclay, MIND team</a>.</span></li>
      <li><span class="date">Jan. 2025</span><span>Visiting Researcher at <a href="https://team.inria.fr/mind/">Inria MIND</a>, studying the link between functional connectivity and cognition with contrastive learning.</span></li>
      <li><span class="date">Dec. 2024</span><span>Became a member of the <a href="https://ellis.eu/">ELLIS Society</a>.</span></li>
      <li><span class="date">Mar. 2024</span><span>Member of the newborn <a href="https://www.aslto3.piemonte.it/azienda/progetti/progetti-aziendali/aslto3-radiomics-lab/">ASL TO3 Radiomics Lab</a> in Rivoli, Italy.</span></li>
    </ul>
    </div>
    <div class="home-pubs">
    <h2>Selected publications</h2>
    <ul>
      <li>
        <span class="title"><a href="https://inria.hal.science/hal-05767107">BrainPFN: Amortized Brain-Behaviour Prediction via Prior-Data Fitted Networks</a></span>
        <span class="meta"><u>C. A. Barbano</u>, D. Wassermann</span>
        <span class="meta"><span class="venue">Preprint</span>, 2026</span>
      </li>
      <li>
        <span class="title"><a href="https://www.sciencedirect.com/science/article/pii/S0167865525003848">Anatomical foundation models for brain MRIs</a></span>
        <span class="meta"><u>C. A. Barbano</u>, M. Brunello, B. Dufumier, M. Grangetto</span>
        <span class="meta"><span class="venue">Pattern Recognition Letters</span>, 2025</span>
      </li>
      <li>
        <span class="title"><a href="https://arxiv.org/abs/2211.08326">Contrastive learning for regression in multi-site brain age prediction</a><span class="badge">Best poster</span></span>
        <span class="meta"><u>C. A. Barbano</u>, B. Dufumier, E. Duchesnay, M. Grangetto, P. Gori</span>
        <span class="meta"><span class="venue">ISBI</span>, 2023</span>
      </li>
      <li>
        <span class="title"><a href="https://arxiv.org/abs/2211.05568">Unbiased Supervised Contrastive Learning</a></span>
        <span class="meta"><u>C. A. Barbano</u>, B. Dufumier, E. Tartaglione, M. Grangetto, P. Gori</span>
        <span class="meta"><span class="venue">ICLR</span>, 2023</span>
      </li>
      <li>
        <span class="title"><a href="https://arxiv.org/abs/2206.01646">Integrating Prior Knowledge in Contrastive Learning with Kernel</a></span>
        <span class="meta">B. Dufumier, <u>C. A. Barbano</u>, R. Louiset, E. Duchesnay, P. Gori</span>
        <span class="meta"><span class="venue">ICML</span>, 2023</span>
      </li>
      <li>
        <span class="title"><a href="https://arxiv.org/abs/2103.02023">EnD: Entangling and Disentangling deep representations for bias correction</a></span>
        <span class="meta">E. Tartaglione, <u>C. A. Barbano</u>, M. Grangetto</span>
        <span class="meta"><span class="venue">CVPR</span>, 2021</span>
      </li>
    </ul>
    <p class="home-more"><a href="/publications/">All publications →</a></p>
    </div>
  </div>
</section>

<section class="home-about">
  <div class="wrap home-cols" markdown="0">
    <div class="home-timeline">
      <h2>Positions</h2>
      <ul>
        <li><span class="when">Nov. 2025 – now</span><strong>Starting Researcher</strong>, <a href="https://team.inria.fr/mind/">Inria Saclay, MIND</a></li>
        <li><span class="when">Jan. – Feb. 2025</span><strong>Visiting Researcher</strong>, <a href="https://team.inria.fr/mind/">Inria MIND</a></li>
        <li><span class="when">Dec. 2023 – Oct. 2025</span><strong>Postdoctoral Researcher</strong>, deep learning for medical imaging, <a href="https://www.unito.it">University of Turin</a></li>
      </ul>
    </div>
    <div class="home-timeline">
      <h2>Education</h2>
      <ul>
        <li><span class="when">2020 – 2023</span><strong>Ph.D. in Computer Science</strong>, <a href="https://www.telecom-paris.fr/en/home">Télécom Paris</a> and <a href="https://www.unito.it">University of Turin</a> (cotutelle). Thesis: <em>Collateral-Free Learning of Deep Representations: From Natural Images to Biomedical Applications</em></li>
        <li><span class="when">2018 – 2020</span><strong>M.Sc. in Artificial Intelligence</strong>, University of Turin</li>
      </ul>
    </div>
  </div>
</section>
