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
  <div class="real-spider-stage" aria-label="Spider-Man floating above a cinematic city backdrop">
    <div class="spider-web-halo" aria-hidden="true"></div>
    <img class="hero-spider-3d" src="https://file.aiquickdraw.com/imgcompressed/img/compressed_8564cf822e167db5111eeb300d836f85.webp" alt="Spider-Man leaping forward and shooting a web">
    <div class="spider-caption"><span>FRIENDLY NEIGHBOURHOOD</span><strong>SPIDER-MAN</strong><small>THWIP! · EARTH-616</small></div>
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

.hero-pose-stack{position:relative;z-index:2;width:min(100%,520px);height:530px}
.real-spider{position:absolute;inset:0;width:100%;height:100%;object-fit:contain;object-position:center bottom;filter:drop-shadow(0 24px 24px rgba(0,0,0,.55))}
.hero-pose{opacity:0;animation:hero-pose-cycle 12s infinite}
.pose-one{animation-delay:0s}.pose-two{animation-delay:4s}.pose-three{animation-delay:8s}
@keyframes hero-pose-cycle{0%,5%{opacity:0;transform:translateY(35px) scale(.94) rotate(-4deg)}10%,27%{opacity:1;transform:translateY(0) scale(1) rotate(0)}33%,100%{opacity:0;transform:translateY(-28px) scale(.96) rotate(5deg)}}
@media(max-width:760px){.hero-pose-stack{height:390px;width:min(100%,390px)}}
@media(prefers-reduced-motion:reduce){.hero-pose{animation:none;opacity:0}.pose-one{opacity:1}}

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

<style>
.journal-hero{grid-template-columns:.92fr 1.08fr;min-height:590px;gap:2%;overflow:hidden}
.real-spider-stage{position:relative;min-height:540px;display:flex;align-items:flex-end;justify-content:center;isolation:isolate}
.real-spider{position:relative;z-index:2;width:min(100%,520px);height:530px;object-fit:contain;object-position:center bottom;filter:drop-shadow(0 24px 24px rgba(0,0,0,.55));animation:spider-hero-arrive 1.1s cubic-bezier(.2,.8,.2,1) both,spider-hero-float 4.5s ease-in-out 1.1s infinite}
.spider-web-halo{position:absolute;z-index:0;width:min(90%,480px);aspect-ratio:1;border-radius:50%;background:radial-gradient(circle,rgba(27,132,218,.28),rgba(229,29,61,.12) 48%,transparent 72%);border:1px solid rgba(105,190,255,.22);box-shadow:0 0 90px rgba(25,132,220,.17)}
.spider-web-halo:before,.spider-web-halo:after{content:"";position:absolute;inset:7%;border:1px solid rgba(120,194,255,.35);border-radius:50%;background:repeating-conic-gradient(from 0deg,transparent 0deg 14deg,rgba(120,194,255,.18) 14.2deg 14.6deg,transparent 14.8deg 30deg)}
.spider-web-halo:after{inset:20%;transform:rotate(15deg)}
.spider-caption{position:absolute;z-index:3;right:0;bottom:35px;display:flex;flex-direction:column;gap:2px;padding:12px 17px;background:rgba(5,13,28,.88);border-left:3px solid #ef2949;box-shadow:5px 6px 0 rgba(25,132,220,.28);transform:rotate(-3deg)}
.spider-caption span,.spider-caption small{font:700 .72rem 'Barlow Condensed',sans-serif;letter-spacing:.18em;color:#79c9ff}
.spider-caption strong{font:400 2rem 'Bangers',cursive;letter-spacing:1px;color:#fff}
@keyframes spider-hero-arrive{from{opacity:0;transform:translateY(60px) scale(.92)}to{opacity:1;transform:translateY(0) scale(1)}}
@keyframes spider-hero-float{0%,100%{translate:0 0}50%{translate:0 -12px}}
@media(max-width:760px){.journal-hero{grid-template-columns:1fr;min-height:0;padding-bottom:30px}.real-spider-stage{min-height:390px;margin-top:-15px}.real-spider{height:390px;width:min(100%,390px)}.spider-caption{right:3%;bottom:12px}}
@media(prefers-reduced-motion:reduce){.real-spider{animation:none}}

/* Let the hero art sit directly in the scene, with no framed/checkerboard panel */
.real-spider-stage{background:transparent!important;border:0!important;box-shadow:none!important}
.hero-spider-3d{background:transparent!important;filter:drop-shadow(0 25px 28px rgba(0,0,0,.55)) drop-shadow(0 0 30px rgba(55,158,255,.24))!important}
.spider-web-halo{background:radial-gradient(circle,rgba(31,130,218,.34),rgba(229,29,61,.12) 45%,transparent 72%)!important;border:0!important;box-shadow:0 0 75px rgba(35,140,235,.18)!important}

/* Use a real alpha-channel cutout, never a checkerboard preview image */
.hero-spider-3d{background:transparent!important;mix-blend-mode:normal!important;object-fit:contain}
.real-spider-stage{background:transparent!important}

/* Static hero for now: no swing, float, or pose cycling */
.hero-spider-3d{animation:none!important;transform:none!important;mix-blend-mode:normal!important;background:transparent!important}
.real-spider-stage:after{animation:none!important}
</style>