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
  <div class="book-stage spider-photo-stage" aria-label="The Spider-Man portrait selected for Shanika's Spider-Verse homepage">
    <div class="spider-web-backdrop" aria-hidden="true">
      <svg viewBox="0 0 520 580" preserveAspectRatio="none">
        <g class="web-lines">
          <path d="M260 12L260 550M20 70L500 510M500 70L20 510M10 290H510M80 18L440 560M440 18L80 560"/>
          <path d="M260 12Q385 100 500 70M260 12Q135 100 20 70M20 70Q90 290 20 510M500 70Q430 290 500 510M20 510Q260 430 500 510M80 18Q260 125 440 18M80 560Q260 450 440 560"/>
          <path d="M160 65Q260 110 360 65M92 140Q260 215 428 140M42 218Q260 310 478 218M33 370Q260 285 487 370M92 455Q260 370 428 455M160 520Q260 465 360 520" class="web-red"/>
        </g>
      </svg>
    </div>
    <div class="spider-photo-halo" aria-hidden="true"></div>
    <span class="spider-photo-cable" aria-hidden="true"></span>
    <figure class="spider-photo-card">
      <img src="{{ '/assets/spider-mask-hero.webp' | relative_url }}" alt="Spider-Man mask portrait chosen for the homepage" width="454" height="680" fetchpriority="high" decoding="async">
      <figcaption><span>EARTH-616 · NEW YORK</span><span>SPIDER-JOURNAL</span></figcaption>
    </figure>
    <svg class="spider-photo-stamp" viewBox="0 0 48 48" aria-hidden="true">
      <g fill="none" stroke="#eaf7ff" stroke-width="2.4" stroke-linecap="round" stroke-linejoin="round">
        <path d="M18 18L8 8M15 23L4 22M17 29L7 38M30 18L40 8M33 23L44 22M31 29L41 38M20 16L15 5M28 16L33 5M20 32L15 43M28 32L33 43"/>
      </g>
      <ellipse cx="24" cy="24" rx="6.3" ry="9" fill="#ed2948"/>
      <circle cx="24" cy="15" r="4.2" fill="#ed2948"/>
    </svg>
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
