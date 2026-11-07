---
layout: default
title: Journal
---

<section class="journal-hero">
  <div class="hero-copy">
    <div class="eyebrow">EARTH-616 · PERSONAL FIELD ARCHIVE</div>
    <h1>Every story leaves a <em>mark.</em></h1>
    <p class="hero-lede">A little universe of things I learn, things I build, books I collect and moments worth remembering. Suit up. Explore the city. Find the stories hidden between the skyscrapers.</p>
    <div class="hero-meta">PLAYER FILE · SHANIKA // WEB-SLINGER IN PROGRESS</div>
    <div class="handwritten" style="margin-top:18px">with great curiosity...</div>
  </div>
  <div class="spider-character-card" aria-hidden="true">
    <svg viewBox="0 0 260 330">
      <defs><linearGradient id="spiderSuitRed" x1="0" x2="1" y1="0" y2="1"><stop stop-color="#ff526b"/><stop offset="1" stop-color="#9d102c"/></linearGradient><linearGradient id="spiderSuitBlue" x1="0" x2="1" y1="0" y2="1"><stop stop-color="#2d9cf0"/><stop offset="1" stop-color="#102a56"/></linearGradient></defs>
      <ellipse cx="133" cy="305" rx="78" ry="12" fill="#000" opacity=".25"/>
      <!-- original spider-hero crouch with one hand shooting a web -->
      <path d="M102 112Q73 92 53 67L34 46Q25 35 16 45L28 68L58 105L83 145Z" fill="url(#spiderSuitRed)" stroke="#ff8292" stroke-width="2"/>
      <path d="M31 48L17 35L7 41L16 58L33 63Z" fill="url(#spiderSuitBlue)" stroke="#63baff" stroke-width="2"/>
      <path d="M157 112L186 79L209 46Q217 34 229 42L222 62L203 103L180 143Z" fill="url(#spiderSuitRed)" stroke="#ff8292" stroke-width="2"/>
      <path d="M222 46L235 30L249 38L243 56L228 64Z" fill="url(#spiderSuitBlue)" stroke="#63baff" stroke-width="2"/>
      <path d="M86 111Q93 80 132 79Q172 83 181 120L169 192L91 194L72 145Z" fill="url(#spiderSuitRed)" stroke="#ff8292" stroke-width="2"/>
      <path d="M93 123L132 143L171 119L168 190L94 194L76 148Z" fill="url(#spiderSuitBlue)" stroke="#63baff" stroke-width="2"/>
      <path d="M91 192L74 237L38 271L54 287L105 260L131 211Z" fill="url(#spiderSuitRed)" stroke="#ff8292" stroke-width="2"/>
      <path d="M151 193L170 232L211 256L198 275L145 258L122 211Z" fill="url(#spiderSuitBlue)" stroke="#63baff" stroke-width="2"/>
      <path d="M94 35Q97 4 132 5Q168 7 171 38L158 83L112 84Z" fill="url(#spiderSuitRed)" stroke="#ff8292" stroke-width="2"/>
      <path d="M108 43Q123 26 135 42L119 58Z" fill="#f4fbff" stroke="#10182a" stroke-width="3"/>
      <path d="M139 42Q155 26 164 43L148 59Z" fill="#f4fbff" stroke="#10182a" stroke-width="3"/>
      <g fill="none" stroke="#ffdce2" stroke-width="1.2" opacity=".8"><path d="M132 8V82M99 19L161 70M163 19L99 70M82 133L132 151L176 130M92 194L132 163L169 194M43 271L57 286M198 258L211 273"/></g>
      <path d="M132 143l-12 18 13 12 13-12z" fill="#fff" stroke="#10182a" stroke-width="2"/>
      <path d="M18 43Q2 24 4 7M18 43Q31 20 42 3M18 43Q-1 45 -13 39" fill="none" stroke="#dff6ff" stroke-width="2" stroke-linecap="round"/>
    </svg>
  </div>
  <div class="book-stage" aria-label="A three-dimensional Spider-Verse field archive">
    <div class="paper-orbit one" aria-hidden="true"></div><div class="paper-orbit two" aria-hidden="true"></div><div class="book-shadow"></div>
    <div class="book">
      <div class="book-back"></div><div class="book-spine"></div><div class="book-pages"></div>
      <div class="book-cover">
        <div class="book-label">CLASSIFIED · FIELD NOTES 001</div>
        <div class="book-title">Into the Webverse.</div>
        <div class="book-mark"><span>SHANIKA // EARTH-616</span><span>✦</span></div>
      </div>
    </div>
    <div class="floating-note"><strong>MISSION LOG</strong>Keep moving. Keep making.</div><div class="handwritten-note">your friendly neighbourhood archive ✦</div>
  </div>
</section>

<section class="web-mission-board reveal" aria-label="Explore the webverse">
  <div class="section-head"><div><div class="eyebrow">Choose your next destination</div><h2>Explore the webverse</h2></div><span class="page-kicker">6 LOCATIONS · 1 UNIVERSE</span></div>
  <div class="web-mission-grid">
    <a href="#all-entries" class="web-mission"><span>01 / MISSIONS</span><strong>Daily Missions</strong><small>Stories, thoughts & memories</small><b>↗</b></a>
    <a href="{{ '/projects/' | relative_url }}" class="web-mission"><span>02 / ARCHIVES</span><strong>The Archives</strong><small>Books & collected stories</small><b>↗</b></a>
    <a href="{{ '/projects/' | relative_url }}" class="web-mission"><span>03 / THE LAB</span><strong>Project Files</strong><small>Experiments & things I build</small><b>↗</b></a>
    <a href="{{ '/about/' | relative_url }}" class="web-mission"><span>04 / PROFILE</span><strong>The Spider File</strong><small>Origin story & abilities</small><b>↗</b></a>
    <a href="{{ '/contact/' | relative_url }}" class="web-mission"><span>05 / COMMS</span><strong>The Web Line</strong><small>Send a signal</small><b>↗</b></a>
    <a href="#all-entries" class="web-mission"><span>06 / CITY LOG</span><strong>Memory Lane</strong><small>Browse the full archive</small><b>↗</b></a>
  </div>
</section>


<style>
.web-mission-board{margin:0 0 76px;padding:28px 0 0;border-top:1px solid rgba(90,151,213,.3)}
.web-mission-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:15px}
.web-mission{position:relative;min-height:145px;padding:20px 22px;text-decoration:none;display:flex;flex-direction:column;align-items:flex-start;justify-content:center;gap:7px;background:linear-gradient(145deg,rgba(20,42,71,.96),rgba(9,18,34,.98));border:1px solid rgba(83,155,221,.4);box-shadow:4px 5px 0 rgba(22,118,200,.17);clip-path:polygon(0 0,95% 0,100% 12%,100% 100%,5% 100%,0 88%);transition:transform .25s,box-shadow .25s,border-color .25s}
.web-mission:hover{transform:translateY(-7px) skewX(-.5deg);border-color:#ef3554;box-shadow:7px 10px 0 rgba(229,29,61,.22)}
.web-mission span{font:600 .78rem 'Barlow Condensed',sans-serif;letter-spacing:.2em;color:#69bfff}
.web-mission strong{font:400 1.9rem 'Bangers',cursive;letter-spacing:1px;color:#fff}
.web-mission small{font:400 1rem 'Barlow Condensed',sans-serif;color:#b4c8e2}
.web-mission b{position:absolute;right:18px;bottom:15px;color:#ff4563;font-size:1.4rem}
@media(max-width:760px){.web-mission-grid{grid-template-columns:1fr 1fr}.web-mission{min-height:130px;padding:16px}}
@media(max-width:420px){.web-mission-grid{grid-template-columns:1fr}}
</style>
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
