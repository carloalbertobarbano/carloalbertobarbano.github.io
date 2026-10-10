---
layout: home
title: "Sitemap"
description: "All pages and publications on the website of Carlo Alberto Barbano."
permalink: /sitemap/
---

<div class="home-narrow" markdown="0">

<header class="page-head">
  <h1>Sitemap</h1>
  <p>All pages and publications on this site. An <a href="/sitemap.xml">XML version</a> is also available.</p>
</header>

<section>
  <h2>Pages</h2>
  <ul class="theme-items">
    <li><a href="/">Home</a></li>
    <li><a href="/research/">Research</a></li>
    <li><a href="/research/brainpfn/">BrainPFN</a></li>
    <li><a href="/research/anatcl/">AnatCL</a></li>
    <li><a href="/research/earlier-work/">Earlier work</a></li>
  </ul>
</section>

<section id="publications">
  <h2>Publications</h2>
  <ul class="theme-items">
    {%- assign pubs = site.publications | sort: "date" | reverse %}
    {%- for p in pubs %}
    <li><a href="{{ p.url }}">{{ p.title }}</a>
      <span class="ref">{{ p.authors | replace: "Carlo Alberto Barbano", "<u>Carlo Alberto Barbano</u>" }} · {{ p.venue }}, {{ p.date | date: "%Y" }}</span></li>
    {%- endfor %}
  </ul>
</section>

</div>
