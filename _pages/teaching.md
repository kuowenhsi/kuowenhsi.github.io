---
layout: page
permalink: /teaching/
title: Teaching
description: Learning to ask questions, evaluate evidence, and think independently.
nav: true
nav_order: 6
calendar: false
_styles: |
  @import url("/assets/css/research.css");
---

<div class="research-page">
<section class="research-intro" aria-labelledby="teaching-philosophy">
<p class="research-kicker">Teaching &amp; Mentoring</p>
<h2 id="teaching-philosophy">Learning how science works</h2>
<p class="research-lead">I help students move beyond knowing biological concepts to understanding how knowledge is generated, tested, and revised.</p>
<p>My teaching combines active learning, scientific reasoning, collaboration, and engagement with primary literature and data. Having taught in Taiwan and the United States, I build in multiple ways for students with different backgrounds and levels of preparation to participate and succeed.</p>
</section>
<nav class="research-jump" aria-label="Teaching sections"><a href="#classroom">In the classroom ↓</a><a href="#mentoring">Research mentoring ↓</a><a href="#courses">Teaching interests ↓</a></nav>

<section id="classroom">
<h2>From biological questions to evidence</h2>
<p>I have taught evolutionary biology, general biology, and botany laboratory courses as a teaching assistant, discussion leader, and laboratory instructor. My experience spans discussion groups of about 15 students and courses of up to 100.</p>
<p>In weekly Evolution discussions at Washington University in St. Louis, I guided students through recent research papers. We started with the biological question and its connection to course concepts before working through hypotheses, experiments, figures, and conclusions.</p>
<ol class="research-steps" aria-label="How we work through a research paper">
<li><span>01 · ASK</span><strong>Find the biological question</strong><p>What are the authors trying to explain, and why does it matter?</p></li>
<li><span>02 · EXAMINE</span><strong>Work with the evidence</strong><p>Interpret figures and datasets, examine the design, and consider alternative explanations.</p></li>
<li><span>03 · DISCUSS</span><strong>Evaluate and revise</strong><p>Explain an interpretation, listen to peers, and refine conclusions in light of the evidence.</p></li>
</ol>
<div class="research-grid">
<div class="research-panel"><h3>Build confidence through collaboration</h3><p>Small-group discussions give students time to organize their ideas before sharing with the class. Peer review of writing helps them practice evaluating scientific arguments and improving their own work through feedback.</p></div>
<div class="research-panel"><h3>Make challenging material accessible</h3><p>Guided paper analysis, clear expectations, and opportunities for revision provide multiple entry points. I also aim to avoid unnecessary financial or technological barriers and support students through office hours and review sessions.</p></div>
</div>
</section>

<section id="mentoring">
<h2>Mentoring toward independence</h2>
<p>I establish goals early, adapt support to each student's experience, and connect research skills with their academic and professional interests. Students participate in the intellectual work of research, from reading literature and interpreting results to communicating their findings.</p>
<div class="research-grid">
<div class="research-panel"><h3>Undergraduate researchers</h3><p>Explore questions and build foundational skills in data collection, analysis, and presentation. Alongside research literacy, I emphasize critical thinking, time management, teamwork, and communication.</p></div>
<div class="research-panel"><h3>Master's students</h3><p>Develop a well-defined project within a larger research program. Achievable milestones support progress through experimental design, analysis, interpretation, and scientific writing.</p></div>
</div>
<div class="research-note"><h3>A vision for doctoral mentoring</h3><p>For Ph.D. students, I envision a progression from smaller projects to questions that reflect their own interests. My goal is to support an independent research identity across proposal development, experimentation, publication, and mentoring junior researchers.</p></div>
<h3>Mentoring experience and outcomes</h3>
<ul>
<li><strong>18 students mentored</strong> across undergraduate and graduate research in Taiwan and the United States.</li>
<li><strong>Eight mentees earned co-authorship</strong> on peer-reviewed publications during my M.S. and Ph.D. training.</li>
<li><strong>Five students received NSF REU funding</strong> at the Missouri Botanical Garden; one Washington University undergraduate received a competitive grant for an independent project.</li>
<li><strong>Two graduate mentees completed M.S. degrees</strong> at National Taiwan University.</li>
</ul>
<p>My aim is a collaborative research environment where students with different backgrounds and career goals can develop expertise, take ownership of their work, and prepare for their next professional stage.</p>
</section>

<section id="courses">
<h2>Teaching interests and course ideas</h2>
<p>I am prepared to contribute to introductory biology and upper-division evolution and genetics. I am also interested in developing courses that combine bioinformatics and AI-assisted computation to investigate plant responses to environmental change.</p>
<p>The course outlines below illustrate additional teaching interests, with an emphasis on primary literature, data analysis, and collaborative problem solving.</p>
<div class="research-grid">
{% assign teaching_outlines = site.teachings | sort: 'importance' %}
{% for course in teaching_outlines %}
{% unless course.title == 'Teaching and mentoring' %}
<a class="research-project" href="{{ course.url | relative_url }}"><div class="research-project-body"><h3>{{ course.title }}</h3><p>{{ course.description }}</p><span class="research-link">Explore the course outline →</span></div></a>
{% endunless %}
{% endfor %}
</div>
</section>
</div>
