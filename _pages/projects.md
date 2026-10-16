---
layout: page
title: projects
permalink: /projects/
description: Research themes and selected projects.
nav: true
nav_order: 3
display_categories: [research]
horizontal: false
---

## Research statement

My research has developed around a central question: how do evolutionary processes determine whether plant populations can persist in changing environments? I address this question by integrating population and conservation genomics, quantitative genetics, common-garden experiments, demographic inference, and historical collections. Across systems ranging from widespread species adapting to climatic gradients to endangered plants undergoing rapid demographic decline and habitat fragmentation, my work seeks to connect genomic variation with phenotype, fitness, and ultimately evolutionary potential.

### Previous and current research

During my Ph.D. at Washington University in St. Louis with Dr. Kenneth Olsen, I used white clover (Trifolium repens) to investigate the genetic basis of rapid and repeated local adaptation. My research identified climate-associated genomic differentiation and demonstrated how different forms of genetic variation contribute to repeatedly evolved adaptive phenotypes. I characterize copy number variation underlying cyanogenesis polymorphism, an ecologically important herbivore defense trait. I also used quantitative genetic mapping to identify the major locus controlling leaf-mark polymorphism and tested whether this phenotype carries a photosynthetic cost. I further investigated the physiological mechanisms underlying cyanogenic adaptation by characterizing the cyanide-detoxification pathway. This work identified a potential compensation mechanism associated with cyanogenesis in cold environments. Complementary drought-stress experiments and gene-expression analyses allowed me to connect adaptive genomic differentiation with phenotypic responses to environmental variation and investigate interactions between homeologous genes in polyploid evolution.

I extended these questions during my postdoctoral research with Dr. Christine Edwards at the Missouri Botanical Garden, where I shifted from widespread systems to endangered plants with small and isolated populations. One recently completed project revealed population connectivity and gene flow interact with disturbance patterns and directly affect genetic diversity and genetic load of plant species in a floodplain ecosystem. A second project addresses a long-standing question in conservation biology: To what extent does present-day population isolation reflect historical biogeographic processes versus recent human-induced habitat fragmentation? I examined this question in Physaria globosa, a federally endangered plant with declining and geographically isolated populations in Kentucky and Tennessee. My analyses revealed deep divergence between the Kentucky and Tennessee populations, extending back approximately one million years, with limited subsequent gene flow. Although recent demographic declines are evident in some populations, substantial genetic diversity and variation in flowering time remain within each regional group. These results suggest that the regional groups have persisted independently while retaining evolutionary potential, raising the possibility of local adaptation. They caution against assuming that genetic mixing is needed or beneficial without testing offspring fitness.

Together, my doctoral and postdoctoral research has positioned me to investigate how population size, connectivity, demographic history, and environmental disturbance influence the capacity for rapid adaptation. This comparative perspective forms the foundation of my independent research program. My training was supported in part by the William H. Danforth Plant Sciences Fellowship and the Taiwan Ministry of Education Studying Abroad Scholarship, which helped me develop independent questions and research plans.

### Future research program

My independent program will ask how population size, structure, connectivity, and demographic history influence the ability of plants to adapt to environmental change, and whether existing variation can support persistence under climate change. In Direction 1, I will compare widespread species with relatively connected populations to habitat-restricted species with patchier distributions across environmental gradients to test how demographic history, standing genetic variation, and gene flow shape local adaptation. In Direction 2, I will use highbush blueberry, a recently domesticated native crop, to test whether genomic regions associated with climate-relevant traits in breeding also vary with climate in wild populations and have changed in frequency over time. Historical herbarium specimens will provide the temporal samples for this test. Together, the two directions connect the mechanisms shaping adaptive variation across space with the pace of evolution under contemporary climate change.

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>

Photo credits: Mimulus — [Eric Johnston](https://commons.wikimedia.org/wiki/File:Mimulus_guttatus.JPG), [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) (resized). Blueberry — [Darkone](https://commons.wikimedia.org/wiki/File:Vaccinium_corymbosum_Beeren.jpg), [CC BY-SA 2.5](https://creativecommons.org/licenses/by-sa/2.5/) (unchanged).
