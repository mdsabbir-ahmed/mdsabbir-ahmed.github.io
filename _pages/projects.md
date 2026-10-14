---
layout: site
title: Projects
permalink: /projects/
nav: true
nav_order: 4
description: Research projects and collaborations.
---
<p class="msa-eyebrow">PROJECTS</p>
<h1 class="msa-page-title">Research projects</h1>
<p class="msa-intro">A selected overview of completed and ongoing research. Projects represent different forms of participation, including principal investigation, co-investigation, study coordination, and collaborative contributions; roles are stated explicitly.</p>
<div class="msa-project-grid msa-projects-page">
{% assign projects_sorted = site.projects | sort: 'importance' %}
{% for project in projects_sorted %}
  <a class="msa-project-card" href="{{ project.url | relative_url }}">
    <span>{{ project.area | default: 'RESEARCH' }}</span>
    <h2>{{ project.title }}</h2>
    <p>{{ project.description }}</p>
    <strong>{{ project.role }} ↗</strong>
  </a>
{% endfor %}
</div>
