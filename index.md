---
layout: default
title: Home
---

<div class="hero">
  <div class="pill">Welcome, Shasha 👋</div>
  <h1>Hey, I'm Shanika – a CSE student exploring AI, web dev & random tech thoughts.</h1>
  <p>This blog is where I document what I learn every day – from Python and machine learning to web projects and college life.</p>
</div>

<section class="posts">
  <h2>Latest Posts</h2>

  {% for post in site.posts %}
  <article class="post-card">
    <a href="{{ post.url | relative_url }}">
      <div class="post-title">{{ post.title }}</div>
      <div class="post-meta">
        {{ post.date | date: "%d %b %Y" }}
      </div>
      <div class="post-excerpt">
        {{ post.excerpt }}
      </div>
    </a>
  </article>
  {% endfor %}

  {% if site.posts == empty %}
  <p class="post-excerpt">No posts yet. Once you add your first post, it will appear here.</p>
  {% endif %}
</section>
