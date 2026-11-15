---
layout: default
title: Journal
---

<section class="journal-hero cinematic-home">
  <div class="hero-copy">
    <div class="eyebrow">EARTH-616 · SHANIKA'S SPIDER-VERSE</div>
    <h1>My own little corner of the <em>Spider-Verse.</em></h1>
    <p class="hero-lede">A personal universe of ideas, books, projects, late-night thoughts and moments worth saving. New York has its friendly neighbourhood Spider-Man. This is my corner of the web.</p>
    <div class="hero-meta">SHANIKA · READER, BUILDER, FRIENDLY NEIGHBOURHOOD OVERTHINKER</div>
    <div class="handwritten" style="margin-top:18px">with great curiosity... and a little responsibility.</div>
  </div>
  <div class="book-stage" aria-label="Interactive three-dimensional red-and-blue Spider-Man inspired mask with a moving webbed suit">
    
  </div>
</section>

<section class="home-recent-feed reveal">
 <div class="section-head">
  <div><div class="eyebrow">Notes from along the way</div><h2>Recently written</h2></div>
 </div>
 <div class="home-post-grid">
 {% for post in site.posts limit:4 %}
 <a class="home-post-card" href="{{ post.url | relative_url }}">
  <div class="home-post-media">
   {% if post.image %}<img src="{{ post.image | relative_url }}" alt="{{ post.title | escape }}" loading="lazy">{% else %}<div class="post-artwork" role="img" aria-label="A red-and-blue Spider-Verse inspired web over a rain-lit New York skyline"><span class="post-art-glow"></span><span class="post-art-web"></span><span class="post-art-silhouette"></span><span class="post-art-label">DAILY BUGLE · PERSONAL EDITION</span></div>{% endif %}
   <span class="feed-date">{{ post.date | date: "%d %B %Y" }}</span>
  </div>
  <div class="home-post-body">
   <div class="home-post-author"><span class="home-post-avatar">S</span> SHANIKA · JOURNAL</div>
   <h3>{{ post.title }}</h3>
   <p>{{ post.excerpt | strip_html | strip | truncate: 135 }}</p>
   <div class="home-post-actions"><span>♡</span><span>READ STORY ↗</span></div>
  </div>
 </a>
 {% else %}
 <div class="empty-note">The next page is waiting to be written.</div>
 {% endfor %}
 </div>
</section>
