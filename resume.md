---
layout: default
title: Resume
description: Resume and profile highlights for James Vashiri.
permalink: /resume/
---

<section class="hero" data-reveal>
  <span class="section-kicker">Career Profile</span>
  <h1>Resume</h1>
  <p>Download or view my resume and review key highlights in education, engineering, AI systems, and research.</p>
  <div class="resume-actions">
    <a class="button" href="{{ site.resume_url | relative_url }}" download>Download Resume</a>
    <a class="button secondary" href="{{ site.resume_url | relative_url }}" target="_blank" rel="noopener">View Resume</a>
  </div>
</section>

<section data-reveal>
  <h2 class="section-title">Embedded Resume Viewer</h2>
  <iframe class="resume-viewer" title="Resume PDF viewer" src="{{ site.resume_url | relative_url }}"></iframe>
  <p class="muted">Upload your resume PDF to the path configured in _config.yml under resume_url.</p>
</section>

<section class="grid-3" data-reveal>
  <article class="card">
    <h3>Education</h3>
    <p class="muted">MS Computer and Information Science at Marquette University, backed by software engineering training.</p>
  </article>
  <article class="card">
    <h3>Technical Depth</h3>
    <p class="muted">AI/ML, TinyML, embedded systems, computer vision, and cybersecurity-informed design.</p>
  </article>
  <article class="card">
    <h3>Research and Impact</h3>
    <p class="muted">Active research roadmap with publication and practical deployment focus.</p>
  </article>
</section>
