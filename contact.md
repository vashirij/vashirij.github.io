---
layout: default
title: Contact
description: Contact James Vashiri for engineering and research collaboration.
permalink: /contact/
---

<section class="hero" data-reveal>
  <span class="section-kicker">Start a Conversation</span>
  <h1>Contact</h1>
  <p>I'm always interested in collaborating on research, AI, embedded systems, and software engineering projects.</p>
</section>

<section class="contact-grid grid-2" data-reveal>
  <article class="contact-card">
    <h3>Contact Form</h3>
    <p class="muted">Use this form for collaboration, recruiter outreach, project consulting, or research opportunities.</p>
    <form action="https://formspree.io/f/your-form-id" method="POST">
      <label for="name">Name</label>
      <input id="name" name="name" type="text" required>

      <label for="email">Email</label>
      <input id="email" name="email" type="email" required>

      <label for="subject">Subject</label>
      <input id="subject" name="subject" type="text" required>

      <label for="message">Message</label>
      <textarea id="message" name="message" required></textarea>

      <button class="button" type="submit">Send Message</button>
    </form>
    <p class="muted">Replace your-form-id with your Formspree endpoint.</p>
  </article>

  <article class="contact-card">
    <h3>Direct Channels</h3>
    <p><strong>Email:</strong> <a href="mailto:james.vashiri@marquette.edu">james.vashiri@marquette.edu</a></p>
    <p><strong>LinkedIn:</strong> <a href="https://linkedin.com/in/jvashiri" target="_blank" rel="noopener">linkedin.com/in/jvashiri</a></p>
    <p><strong>GitHub:</strong> <a href="https://github.com/vashirij" target="_blank" rel="noopener">github.com/vashirij</a></p>
    <p><strong>Location:</strong> Milwaukee, WI</p>

    <h3 style="margin-top: 1.5rem;">Call to Action</h3>
    <p class="muted">I am open to software engineering, AI/ML, embedded systems, and research roles, including opportunities that bridge industry and academic innovation.</p>
    <div class="hero-actions">
      <a class="button secondary" href="{{ '/projects/' | relative_url }}">Explore Projects</a>
      <a class="button ghost" href="{{ '/research/' | relative_url }}">View Research</a>
    </div>
  </article>
</section>
