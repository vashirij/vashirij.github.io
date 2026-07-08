---
layout: default
title: Publications
description: Publication timeline and research output by James Vashiri.
permalink: /publications/
---

<section data-reveal>
  <span class="section-kicker">Research Output</span>
  <h1 class="section-title" style="margin-top: 0;">Publications</h1>
  <p class="muted">Conference papers, journal manuscripts, surveys, posters, and in-preparation work in AI systems and embedded intelligence.</p>
</section>

<section class="publication-list" data-reveal>
  {% for paper in site.data.publications %}
  <article class="publication-card">
    <p class="status">{{ paper.status }} | {{ paper.venue_type }}</p>
    <h3>{{ paper.title }}</h3>
    <p class="muted">{{ paper.authors }}</p>
    <p>{{ paper.venue }}</p>
    <div class="tag-list">
      <span class="tag">{{ paper.year }}</span>
      <span class="tag">{{ paper.category }}</span>
    </div>
    <div class="hero-actions" style="margin-top: 0.8rem;">
      <a class="button secondary" href="{{ paper.pdf }}" target="_blank" rel="noopener">PDF</a>
      <a class="button ghost" href="{{ paper.bibtex }}" target="_blank" rel="noopener">BibTeX</a>
      <a class="button ghost" href="{{ paper.citation }}" target="_blank" rel="noopener">Citation</a>
      <a class="button ghost" href="{{ paper.doi }}" target="_blank" rel="noopener">DOI</a>
      <a class="button ghost" href="{{ paper.github }}" target="_blank" rel="noopener">GitHub</a>
    </div>
  </article>
  {% endfor %}
</section>
