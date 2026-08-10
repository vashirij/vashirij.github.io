---
layout: default
title: James Vashiri
description: James Vashiri is a Software Engineer building intelligent systems across AI, computer vision, embedded systems, and edge computing.
permalink: /
---

<section class="hero" data-reveal>
  <span class="section-kicker">Software Engineer Portfolio</span>
  <h1>James Vashiri</h1>
  <p class="subtitle">Software Engineer | AI and Machine Learning | Computer Vision | Embedded Systems</p>
  <p>I build intelligent systems that combine AI, embedded computing, cybersecurity, and software engineering to solve practical engineering problems in real-world environments.</p>

  <div class="hero-actions">
    <a class="button" href="{{ '/projects/' | relative_url }}">View Projects</a>
    <a class="button secondary" href="{{ '/resume/' | relative_url }}">Download Resume</a>
    <a class="button ghost" href="{{ '/contact/' | relative_url }}">Contact Me</a>
  </div>

  <div class="social-links">
    <a href="https://github.com/vashirij" target="_blank" rel="noopener"><i class="fa-brands fa-github"></i> GitHub</a>
    <a href="https://linkedin.com/in/jvashiri" target="_blank" rel="noopener"><i class="fa-brands fa-linkedin"></i> LinkedIn</a>
    <a href="https://scholar.google.com" target="_blank" rel="noopener"><i class="fa-solid fa-graduation-cap"></i> Google Scholar</a>
    <a href="mailto:james.vashiri@marquette.edu"><i class="fa-solid fa-envelope"></i> Email</a>
  </div>

  <div class="tech-icons">
    <span><i class="fa-brands fa-python"></i> Python</span>
    <span><i class="fa-solid fa-superscript"></i> MATLAB</span>
    <span><i class="fa-solid fa-code"></i> C++</span>
    <span><i class="fa-brands fa-linux"></i> Linux</span>
    <span><i class="fa-solid fa-brain"></i> TensorFlow</span>
    <span><i class="fa-brands fa-git-alt"></i> Git</span>
    <span><i class="fa-brands fa-docker"></i> Docker</span>
  </div>
</section>

<section data-reveal>
  <h2 class="section-title">Technical Skills</h2>
  <p class="muted">A focused systems profile spanning software, AI research, and deployable edge intelligence.</p>
  <div class="skill-grid">
    {% for skill in site.data.skills.languages %}
    <article class="skill-card">
      <h3>{{ skill.name }}</h3>
      <p class="muted">Language</p>
      <div class="skill-meter"><span style="width: {{ skill.level }}%"></span></div>
    </article>
    {% endfor %}
  </div>
  <div class="skill-grid" style="margin-top: 1rem;">
    {% for skill in site.data.skills.technologies %}
    <article class="skill-card">
      <h3>{{ skill.name }}</h3>
      <p class="muted">Technology</p>
      <div class="skill-meter"><span style="width: {{ skill.level }}%"></span></div>
    </article>
    {% endfor %}
  </div>
</section>

<section data-reveal>
  <h2 class="section-title">Featured Projects</h2>
  <div class="card-grid">
    {% for project in site.data.projects limit:6 %}
    <article class="project-card" data-filter-card data-tags="{{ project.tags | join: ' ' | downcase }}">
      <img class="project-thumb" loading="lazy" src="{{ project.image | relative_url }}" alt="{{ project.title }} preview image">
      <h3>{{ project.title }}</h3>
      <p class="muted">{{ project.description }}</p>
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

<section class="card" data-reveal>
  <h2 class="section-title">Recruiter Snapshot</h2>
  <div class="grid-3">
    <div>
      <h3>Research Depth</h3>
      <p class="muted">TinyML, edge intelligence, AI security, and cyber-physical systems with publication and roadmap focus.</p>
    </div>
    <div>
      <h3>Engineering Delivery</h3>
      <p class="muted">From embedded and IoT platforms to software systems and computer vision pipelines.</p>
    </div>
    <div>
      <h3>Career Direction</h3>
      <p class="muted">Open to software engineering, AI/ML, embedded systems, and research opportunities including PhD pathways.</p>
    </div>
  </div>
</section>
