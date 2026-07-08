---
layout: default
title: Projects
description: Engineering and AI projects by James Vashiri.
permalink: /projects/
---

<section data-reveal>
  <span class="section-kicker">Engineering Portfolio</span>
  <h1 class="section-title" style="margin-top: 0;">Projects</h1>
  <p class="muted">A project set spanning AI, machine learning, embedded systems, MATLAB analytics, IoT, and security.</p>
</section>

<section data-reveal>
  <div class="filter-controls" role="toolbar" aria-label="Project filters">
    <button class="active" data-filter-button="all">All</button>
    <button data-filter-button="ai">AI</button>
    <button data-filter-button="machine learning">Machine Learning</button>
    <button data-filter-button="embedded">Embedded</button>
    <button data-filter-button="computer vision">Computer Vision</button>
    <button data-filter-button="iot">IoT</button>
    <button data-filter-button="cybersecurity">Cybersecurity</button>
    <button data-filter-button="matlab">MATLAB</button>
    <button data-filter-button="python">Python</button>
  </div>

  <div class="card-grid">
    {% for project in site.data.projects %}
    <article class="project-card" data-filter-card data-tags="{{ project.tags | join: ' ' | downcase }}" data-reveal>
      <img class="project-thumb" loading="lazy" src="{{ project.image | relative_url }}" alt="{{ project.title }} image">
      <h3>{{ project.title }}</h3>
      <p>{{ project.description }}</p>
      <div class="tag-list">
        {% for tag in project.tags %}
        <span class="tag">{{ tag }}</span>
        {% endfor %}
      </div>
      <div class="hero-actions">
        <a class="button secondary" href="{{ project.github }}" target="_blank" rel="noopener">GitHub</a>
        {% if project.demo %}
        <a class="button ghost" href="{{ project.demo }}" target="_blank" rel="noopener">Live Demo</a>
        {% endif %}
      </div>
    </article>
    {% endfor %}
  </div>
</section>
