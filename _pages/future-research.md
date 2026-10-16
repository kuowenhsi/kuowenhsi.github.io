---
layout: page
title: Future Research Plans
permalink: /future-research/
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
<a href="#directions">Explore the two directions ↓</a><a href="{{ "/projects/" | relative_url }}">Current and Previous Projects →</a>
</nav>
<section id="directions">
<h2>Two directions, one central question</h2>
<p>My future program connects the distribution of adaptive variation across landscapes with the pace of evolution through time.</p>
<div class="research-grid">
{% assign future_projects = site.projects | where: "research_group", "future" | sort: "importance" %}
{% for project in future_projects %}
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
</div>
