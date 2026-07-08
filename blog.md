---
layout: default
title: Blog
description: Technical writing by James Vashiri.
permalink: /blog/
---

<section class="hero" data-reveal>
  <span class="section-kicker">Technical Writing</span>
  <h1>Blog</h1>
  <p>Engineering notes and research reflections on machine learning, TinyML, MATLAB, computer vision, Python, and systems engineering.</p>
  <div class="tag-list">
    <span class="tag">Machine Learning</span>
    <span class="tag">TinyML</span>
    <span class="tag">MATLAB</span>
    <span class="tag">Computer Vision</span>
    <span class="tag">Python</span>
    <span class="tag">Research</span>
    <span class="tag">Engineering</span>
  </div>
</section>

<section data-reveal>
  <h2 class="section-title">Featured Articles</h2>
  <div class="grid-2">
    {% assign featured_posts = site.posts | where: 'featured', true %}
    {% if featured_posts.size > 0 %}
      {% for post in featured_posts limit: 4 %}
      <article class="blog-card">
        <p class="meta-row">{{ post.date | date: '%B %d, %Y' }} | Featured</p>
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p class="muted">{{ post.excerpt | strip_html | truncate: 160 }}</p>
        <a class="button ghost" href="{{ post.url | relative_url }}">Read Article</a>
      </article>
      {% endfor %}
    {% else %}
      <article class="blog-card">
        <h3>No featured posts yet</h3>
        <p class="muted">Create markdown posts in _posts and set featured: true in front matter to surface them here.</p>
      </article>
    {% endif %}
  </div>
</section>

<section data-reveal>
  <h2 class="section-title">All Articles</h2>
  <div class="grid-2">
    {% for post in site.posts %}
    <article class="blog-card">
      <p class="meta-row">{{ post.date | date: '%B %d, %Y' }}</p>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p class="muted">{{ post.excerpt | strip_html | truncate: 180 }}</p>
      <a class="button ghost" href="{{ post.url | relative_url }}">Read Article</a>
    </article>
    {% endfor %}
  </div>
</section>
