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
  <div class="book-stage spider-photo-stage" aria-label="Shanika's animated Spider-Verse mask emblem">
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
    <span class="spider-3d-orbit orbit-one" aria-hidden="true"></span>
    <span class="spider-3d-orbit orbit-two" aria-hidden="true"></span>
    <span class="spider-3d-spark spark-one" aria-hidden="true"></span>
    <span class="spider-3d-spark spark-two" aria-hidden="true"></span>
    <span class="spider-hero-particle particle-three" aria-hidden="true"></span>
    <span class="spider-hero-particle particle-four" aria-hidden="true"></span>
    <span class="spider-hero-particle particle-five" aria-hidden="true"></span>
    <span class="spider-hero-scan" aria-hidden="true"></span>
    <div class="spider-card-shell">
      <div class="spider-mask-open" aria-label="Animated Spider-Verse mask artwork">
        <figure class="spider-photo-card">
          <img class="spider-mask-art" src="{{ '/assets/spider-mask-direct.png' | relative_url }}" alt="Red webbed mask emblem with white eyes" width="368" height="528" fetchpriority="high" decoding="async">
          <figcaption><span>EARTH-616 · NEW YORK</span><span>SPIDER-JOURNAL</span></figcaption>
        </figure>
      </div>
</div>
    <span class="spider-depth-shard shard-one" aria-hidden="true"></span>
    <span class="spider-depth-shard shard-two" aria-hidden="true"></span>
    <span class="spider-depth-shard shard-three" aria-hidden="true"></span>
    <span class="spider-stage-light" aria-hidden="true"></span>
<svg class="spider-photo-stamp" viewBox="0 0 48 48" aria-hidden="true">
      <g fill="none" stroke="#eaf7ff" stroke-width="2.4" stroke-linecap="round" stroke-linejoin="round">
        <path d="M18 18L8 8M15 23L4 22M17 29L7 38M30 18L40 8M33 23L44 22M31 29L41 38M20 16L15 5M28 16L33 5M20 32L15 43M28 32L33 43"/>
      </g>
      <ellipse cx="24" cy="24" rx="6.3" ry="9" fill="#ed2948"/>
      <circle cx="24" cy="15" r="4.2" fill="#ed2948"/>
    </svg>
  </div>
</section>

<section class="home-recent-feed reveal" id="missions-feed">
 <div class="section-head">
  <div><div class="eyebrow">Transmission log · Earth-616</div><h2>Recently written</h2></div>
  <span class="ig-feed-count">FIELD NOTES / 04</span>
 </div>
 <div class="ig-feed-layout">
  <div class="home-post-grid">
  {% for post in site.posts limit:4 %}
  {% assign social_id = post.url | slugify %}
  <article class="home-post-card" id="feed-{{ social_id }}" data-social-post data-post-id="{{ social_id }}">
   <header class="ig-post-header">
    <div class="ig-author-block">
     <span class="home-post-avatar" aria-hidden="true">S</span>
     <span class="ig-author-copy"><strong>SHANIKA</strong><small>EARTH-616 · PERSONAL FEED</small></span>
    </div>
    <time class="ig-post-date" datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%d %b %Y" }}</time>
   </header>
   <a class="ig-image-link" href="{{ post.url | relative_url }}" aria-label="Open {{ post.title | escape }}">
    <div class="home-post-media">
     {% if post.image %}<img src="{{ post.image | relative_url }}" alt="{{ post.image_alt | default: post.title | escape }}" loading="lazy" decoding="async">{% else %}<div class="post-artwork" role="img" aria-label="A midnight city skyline crossed by glowing web lines"><span class="post-art-glow"></span><span class="post-art-web"></span><span class="post-art-silhouette"></span><span class="post-art-label">DAILY BUGLE · PERSONAL EDITION</span></div>{% endif %}
     <span class="feed-date">ISSUE / {{ forloop.index | prepend: "00" | slice: -2, 2 }}</span>
     <span class="ig-image-corner" aria-hidden="true">↗</span>
    </div>
   </a>
   <div class="home-post-body">
    <div class="ig-post-toolbar">
     <button class="ig-icon-button ig-like-button" type="button" data-like aria-pressed="false" aria-label="Like this post">
      <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M20.8 4.7a5.5 5.5 0 0 0-7.8 0L12 5.8l-1.1-1.1a5.5 5.5 0 0 0-7.8 7.8l1.1 1.1L12 21l7.8-7.4 1.1-1.1a5.5 5.5 0 0 0-.1-7.8Z"/></svg>
      <span>LIKE</span>
     </button>
     <button class="ig-icon-button" type="button" data-comment-toggle aria-expanded="false" aria-controls="comments-{{ social_id }}">
      <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M20 11.5a7.5 7.5 0 0 1-8 7.5 8.8 8.8 0 0 1-3.5-.7L4 20l1.2-3.5A7.1 7.1 0 0 1 4 12c0-4.2 3.6-7.5 8-7.5s8 2.8 8 7Z"/></svg>
      <span>COMMENT <small data-comment-count>0</small></span>
     </button>
     <a class="ig-read-link" href="{{ post.url | relative_url }}">READ POST <b>↗</b></a>
    </div>
    <p class="ig-likes-line" data-likes-line aria-live="polite">Be the first to send this post some love.</p>
    <div class="ig-caption">
     <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
     <p>{{ post.excerpt | strip_html | strip | truncate: 190 }}</p>
    </div>
    <section class="ig-comments-panel" id="comments-{{ social_id }}" data-comments-panel hidden>
     <div class="ig-comment-list" data-comment-list aria-live="polite">
      <p class="ig-empty-comments">No comments yet. Start the conversation.</p>
     </div>
     <form class="ig-comment-form" data-comment-form>
      <label class="visually-hidden" for="comment-{{ social_id }}">Write a comment</label>
      <input id="comment-{{ social_id }}" name="comment" type="text" maxlength="280" autocomplete="off" placeholder="Add a comment to the web..." required>
      <button type="submit">POST</button>
     </form>
     <p class="ig-local-note">Comments and likes are saved in this browser.</p>
    </section>
   </div>
  </article>
  {% else %}
  <div class="empty-note">The next page is waiting to be written.</div>
  {% endfor %}
  </div>
  <aside class="ig-post-index" aria-label="Post index">
   <div class="ig-index-heading"><small>YOUR FIELD ARCHIVE</small><strong>JUMP TO A POST</strong></div>
   <ol>
    {% for post in site.posts limit:4 %}
    <li>
     <a href="{{ post.url | relative_url }}" data-post-index-link="{{ post.url | slugify }}">
      <span class="ig-index-number">{{ forloop.index | prepend: "00" | slice: -2, 2 }}</span>
      <span class="ig-index-copy"><strong>{{ post.title }}</strong><small>{{ post.date | date: "%d %b %Y" }}</small></span>
      <b aria-hidden="true">↗</b>
     </a>
    </li>
    {% endfor %}
   </ol>
   <p class="ig-index-footnote">SELECT AN ISSUE TO OPEN ITS FULL STORY.</p>
  </aside>
 </div>
</section>
  </div>
 </article>
 {% else %}
 <div class="empty-note">The next page is waiting to be written.</div>
 {% endfor %}
 </div>
</section>
