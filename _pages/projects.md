---
layout: page
title: Current and Previous Projects
permalink: /projects/
description: Plant adaptation, population genetics, and conservation genomics.
nav: true
nav_order: 4
_styles: |
  @import url("/assets/css/research.css");
---

<div class="research-page">
<p class="research-lead">Connecting evolutionary processes with the persistence of plant populations.</p>
<nav class="research-jump" aria-label="Project sections"><a href="#existing-projects">Explore projects ↓</a><a href="{{ '/future-research/' | relative_url }}">Future Research Plans →</a></nav>
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
<h2>Explore the projects</h2>
<div class="research-grid">
{% assign existing_projects = site.projects | where: "research_group", "current_previous" | sort: "importance" %}
{% for project in existing_projects %}
<a class="research-project" href="{{ project.url | relative_url }}">
<div class="research-project-body"><h3>{{ project.title }}</h3><p>{{ project.description | markdownify | remove: '<p>' | remove: '</p>' }}</p><span class="research-link">Read about this project →</span></div>
</a>
{% endfor %}
</div>
</section>
</div>
