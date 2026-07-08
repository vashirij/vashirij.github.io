---
layout: default
title: About
description: About James Vashiri.
permalink: /about/
---

<section class="hero" data-reveal>
  <span class="section-kicker">Professional Profile</span>
  <h1>About</h1>
  <p>Master's student in Computer and Information Science at Marquette University with a software engineering foundation and active research in AI, machine learning, embedded systems, computer vision, IoT, and cybersecurity.</p>
  <p>I focus on solving real engineering problems with mathematically grounded models and deployable intelligent systems.</p>
</section>

<section data-reveal>
  <h2 class="section-title">Education, Experience, and Research Timeline</h2>
  <div class="timeline">
    {% for item in site.data.timeline %}
    <article class="timeline-item">
      <p class="period">{{ item.period }} | {{ item.type }}</p>
      <h3>{{ item.title }}</h3>
      <p class="muted">{{ item.organization }}</p>
      <p>{{ item.description }}</p>
    </article>
    {% endfor %}
  </div>
</section>

<section class="card" data-reveal>
  <h2 class="section-title">Focus Areas</h2>
  <div class="grid-3">
    <div>
      <h3>AI and Machine Learning</h3>
      <p class="muted">Model design, adaptation, and practical deployment pipelines for intelligent systems.</p>
    </div>
    <div>
      <h3>Embedded and IoT Systems</h3>
      <p class="muted">Edge computing workflows for resource-constrained environments and connected systems.</p>
    </div>
    <div>
      <h3>Security and Reliability</h3>
      <p class="muted">Cybersecurity-aware AI design with robust and explainable behavior under real constraints.</p>
    </div>
  </div>
</section>
