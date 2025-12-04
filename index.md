---
layout: default
title: Home
---

<div class="hero">
  <div class="left">
    <div class="tech-badge">
      <div class="tech-dot" aria-hidden="true"></div>
      <div style="font-weight:600;">Student • Developer</div>
    </div>

    <h1>Hi — I'm Shanika. I document what I learn about AI, web development and software engineering.</h1>
    <p>Short technical notes, project updates and practical code experiments. Content focused on learning, building and sharing practical solutions.</p>
  </div>

  <div class="visual" aria-hidden="true">
    <!-- decorative grid dots -->
    <div class="grid-dot" style="left:12%; top:18%;"></div>
    <div class="grid-dot" style="left:30%; top:40%;"></div>
    <div class="grid-dot" style="left:64%; top:22%;"></div>
    <div class="grid-dot" style="left:78%; top:68%;"></div>
  </div>
</div>

<section style="margin-top:6px;">
  <div class="page-header">
    <h2>Latest posts</h2>
    <div class="muted">Recent technical notes and project write-ups</div>
  </div>

  <div style="height:12px"></div>

  {% assign posts_list = site.posts %}
  {% if posts_list and posts_list != empty %}
  <div class="posts-grid">
    {% for post in posts_list %}
    <a class="post-card" href="{{ post.url | relative_url }}">
      <div class="post-visual">
        {% if post.image %}
          <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
        {% else %}
          <!-- no image: use a CSS background gradient; leave the element empty so CSS gradient shows -->
        {% endif %}
        <div class="post-overlay">
          <h3 class="post-title">{{ post.title }}</h3>
          <div class="post-meta">{{ post.date | date: "%d %b %Y" }}</div>
        </div>
      </div>

      <div class="post-body">
        {{ post.excerpt | strip_html | truncate: 120 }}
      </div>
    </a>
    {% endfor %}
  </div>
  {% else %}
  <p class="muted">No posts yet. Add a post under <code>_posts/</code> and it will appear here.</p>
  {% endif %}
</section>
