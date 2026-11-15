---
layout: default
title: Journal
---

<section class="journal-hero cinematic-home">
  <div class="hero-copy">
    <div class="eyebrow">A PERSONAL UNIVERSE · EARTH-616</div>
    <h1>Every story leaves a <em>mark.</em></h1>
    <p class="hero-lede">Things I learn, things I build, books I collect and moments worth remembering. A little corner of the city that is entirely mine.</p>
    <div class="hero-meta">SHANIKA · BUILDER, READER, WORK IN PROGRESS</div>
    <div class="handwritten" style="margin-top:18px">with great curiosity...</div>
  </div>
  <div class="book-stage" aria-label="Interactive three-dimensional masked superhero portrait">
    <div class="hero-scene-backdrop"></div>
  </div>
</section>

<section class="home-recent-feed reveal">
 <div class="section-head">
  <div><div class="eyebrow">Notes from along the way</div><h2>Recently written</h2></div>
 </div>
 <div class="home-post-grid">
 {% for post in site.posts limit:3 %}
 <a class="home-post-card" href="{{ post.url | relative_url }}">
  <div class="home-post-media">
   {% if post.image %}<img src="{{ post.image | relative_url }}" alt="{{ post.title | escape }}" loading="lazy">{% else %}<div class="post-artwork" role="img" aria-label="Cinematic midnight city artwork with a red and blue web motif"><span class="post-art-glow"></span><span class="post-art-web"></span><span class="post-art-silhouette"></span><span class="post-art-label">FIELD NOTES · 616</span></div>{% endif %}
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
