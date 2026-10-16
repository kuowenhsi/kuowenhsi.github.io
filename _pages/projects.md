---
layout: page
title: projects
permalink: /projects/
description: How plants adapt, persist, and evolve in changing environments.
nav: true
nav_order: 3
_styles: |
  @import url("/assets/css/research.css");
---

<div class="research-page">
<section class="research-intro" aria-labelledby="research-statement">
<p class="research-kicker">Evolution · Genomics · Conservation</p>
<h2 id="research-statement">Research statement</h2>
<p class="research-lead">What gives plant populations the capacity to persist in a changing environment?</p>
<p>I study how population history, genetic variation, and gene flow shape adaptation. My work connects genomes to traits and fitness—from widespread plants adapting across climatic gradients to endangered species surviving in small, isolated populations.</p>
<p>I combine population genomics, common-garden experiments, quantitative genetics, and historical collections to understand both the potential for adaptation and its limits.</p>
</section>
<nav class="research-jump" aria-label="Research sections">
<a href="#directions">Future directions ↓</a><a href="#foundation">Research foundation ↓</a><a href="#existing-projects">Existing projects ↓</a>
</nav>
<section id="directions">
<h2>Two directions, one central question</h2>
<p>My future program connects the distribution of adaptive variation across landscapes with the pace of evolution through time.</p>
<div class="research-grid">
{% assign future_projects = site.projects | sort: "importance" %}
{% for project in future_projects limit:2 %}
<a class="research-project" href="{{ project.url | relative_url }}">
<img src="{{ project.img | relative_url }}" alt="{{ project.image_alt }}" width="{{ project.image_width }}" height="{{ project.image_height }}" loading="lazy">
<div class="research-project-body">
<p class="research-kicker">Direction {{ project.importance }}</p>
<h3>{{ project.title }}</h3>
<p>{{ project.description }}</p>
<span class="research-link">Explore this direction →</span>
</div>
</a>
{% endfor %}
</div>
<p class="research-photo-credit"><small>Photos: Mimulus by <a href="https://commons.wikimedia.org/wiki/File:Mimulus_guttatus.JPG">Eric Johnston</a>, <a href="https://creativecommons.org/licenses/by-sa/3.0/">CC BY-SA 3.0</a> (resized); blueberry by <a href="https://commons.wikimedia.org/wiki/File:Vaccinium_corymbosum_Beeren.jpg">Darkone</a>, <a href="https://creativecommons.org/licenses/by-sa/2.5/">CC BY-SA 2.5</a> (unchanged).</small></p>
</section>
<section id="foundation">
<h2>From adaptive traits to conservation decisions</h2>
<div class="research-grid">
<div class="research-panel">
<h3>How widespread plants adapt</h3>
<p>My doctoral research used white clover to connect climatic adaptation with genomic variation, chemical defense, leaf patterns, and drought responses. It established a foundation for studying how different genetic mechanisms produce adaptive traits.</p>
</div>
<div class="research-panel">
<h3>How rare plants persist</h3>
<p>My postdoctoral work examines how disturbance, isolation, and population history shape endangered plants. In <em>Physaria globosa</em>, deeply divergent regional groups retain genetic and flowering-time variation—highlighting why the benefits of genetic mixing need to be tested.</p>
</div>
</div>
</section>
<section id="existing-projects">
<h2>Existing projects</h2>
<div class="research-grid">
{% assign existing_projects = site.projects | sort: "importance" %}
{% for project in existing_projects offset:2 %}
<a class="research-project" href="{{ project.url | relative_url }}">
<div class="research-project-body"><h3>{{ project.title }}</h3><p>{{ project.description | markdownify | remove: '<p>' | remove: '</p>' }}</p><span class="research-link">Read about this project →</span></div>
</a>
{% endfor %}
</div>
</section>
</div>
