---
layout: default
title: Journal
---

<section class="journal-hero">
  <div class="hero-copy">
    <div class="eyebrow">A personal archive · Since 2025</div>
    <h1>Somewhere between <em>thoughts</em> and things I build.</h1>
    <p class="hero-lede">A little corner of the internet for things I learn, things I make, and moments I want to remember. Part engineering notebook, part personal journal. Always a work in progress.</p>
    <div class="hero-meta">Notes from Shanika's world</div><div class="handwritten" style="margin-top:18px">written as I go...</div>
  </div>
  <div class="book-stage" aria-label="A three-dimensional journal cover">
    <div class="paper-orbit one" aria-hidden="true"></div><div class="paper-orbit two" aria-hidden="true"></div><div class="book-shadow"></div>
    <div class="book">
      <div class="book-back"></div><div class="book-spine"></div><div class="book-pages"></div>
      <div class="book-cover">
        <div class="book-label">Volume 01 · Personal archive</div>
        <div class="book-title">The things I'm figuring out.</div>
        <div class="book-mark"><span>Shanika's journal</span><span>✳</span></div>
      </div>
    </div>
    <div class="floating-note"><strong>Dear future me,</strong>keep noticing things.</div><div class="handwritten-note">little things matter ✳</div>
  </div>
</section>

<section class="reveal">
  <div class="section-head">
    <div><div class="eyebrow">The latest entries</div><h2>Recently written</h2></div>
    <a class="text-link" href="#all-entries">Browse the pages ↓</a>
  </div>
  <div class="entries">
    {% for post in site.posts limit:3 %}
    <a class="entry" href="{{ post.url | relative_url }}">
      <div class="entry-date">{{ post.date | date: "%d %B %Y" }}</div>
      <h3>{{ post.title }}</h3>
      <p>{{ post.excerpt | strip_html | strip | truncate: 120 }}</p>
      <span class="entry-arrow">↗</span>
    </a>
    {% else %}
    <div class="empty-note">The next page is waiting to be written.</div>
    {% endfor %}
  </div>
</section>

<section class="reveal" id="all-entries" style="margin-top:76px">
  <div class="section-head">
    <div><div class="eyebrow">Everything, in its own time</div><h2>From the archive</h2></div>
    <span class="page-kicker">{{ site.posts.size }} entries</span>
  </div>
  <div class="post-list">
    {% for post in site.posts %}
    <a class="post-row" href="{{ post.url | relative_url }}"><span>{{ post.title }}</span><span>{{ post.date | date: "%d · %b · %Y" }}</span></a>
    {% else %}
    <p>Nothing here yet. That's part of keeping a journal.</p>
    {% endfor %}
  </div>
</section>
