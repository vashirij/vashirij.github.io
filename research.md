---
layout: default
title: Research
description: Research vision and roadmap by James Vashiri.
permalink: /research/
---

<section class="hero" data-reveal>
  <span class="section-kicker">Research Program</span>
  <h1>Research</h1>
  <p>My research vision is to build adaptive and trustworthy intelligence at the edge, where machine learning systems can operate securely, efficiently, and reliably in cyber-physical environments.</p>
</section>

<section data-reveal>
  <h2 class="section-title">Current Interests</h2>
  <div class="grid-3">
    {% for interest in site.data.research.interests %}
    <article class="card">
      <h3>{{ interest.title }}</h3>
      <p class="muted">{{ interest.summary }}</p>
    </article>
    {% endfor %}
  </div>
</section>

<section data-reveal>
  <h2 class="section-title">Current Projects</h2>
  <div class="grid-2">
    {% for project in site.data.research.current_projects %}
    <article class="card">
      <h3>{{ project.title }}</h3>
      <p>{{ project.summary }}</p>
      <p class="muted">{{ project.stage }}</p>
    </article>
    {% endfor %}
  </div>
</section>

<section data-reveal>
  <h2 class="section-title">Research Roadmap</h2>
  <div class="timeline">
    {% for step in site.data.research.roadmap %}
    <article class="timeline-item">
      <p class="period">{{ step.period }}</p>
      <h3>{{ step.title }}</h3>
      <p class="muted">{{ step.outcome }}</p>
    </article>
    {% endfor %}
  </div>
</section>

<section class="card" data-reveal>
  <h2 class="section-title">Future Directions</h2>
  <div class="grid-2">
    {% for direction in site.data.research.future_directions %}
    <div>
      <h3>{{ direction.title }}</h3>
      <p class="muted">{{ direction.summary }}</p>
    </div>
    {% endfor %}
  </div>
</section>
