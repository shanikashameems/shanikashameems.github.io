---
layout: default
title: Home
---

<!-- DESCRIPTION CONTAINER -->
<section style="
  margin-top:12px; /* GAP BETWEEN NAVBAR AND DESCRIPTION */
  border:1px solid rgba(255,255,255,0.05);
  padding:48px;
  border-radius:14px;
  background:linear-gradient(180deg, rgba(13,17,28,0.55), rgba(6,8,14,0.32));
  backdrop-filter:blur(12px);

  /* ANIMATION APPLIED TO WHOLE DESCRIPTION CONTAINER */
  opacity:0;
  animation:descContainerAnim 1s ease forwards;
">
  <div style="
    font-size:.8rem;
    text-transform:uppercase;
    letter-spacing:2px;
    margin:0 0 25px 0;
    background:linear-gradient(90deg,#3b82f6,#7c3aed);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
    font-weight:600;
  ">
    Shanika S · Engineering Notebook
  </div>

  <h1 style="
    margin:0 0 14px 0;
    font-size:1.95rem;
    font-weight:700;
    letter-spacing:-0.02em;
  ">
    I build software, explore machine intelligence, and document my journey in public.
  </h1>

  <p style="
    color:#9ca3af;
    max-width:680px;
    font-size:1.05rem;
    margin:0;
  ">
    I’m a Computer Science student focused on AI and full-stack engineering.
    This space captures the systems I build, the concepts I study, and the ideas that shape my work.
  </p>
</section>


<!-- SPACE BEFORE POSTS -->
<div style="height:24px;"></div>


<!-- POSTS HEADER (unchanged) -->
<div style="
  display:flex;
  align-items:center;
  justify-content:space-between;
">
  <h2 style="margin:0; font-size:1.32rem; font-weight:600;">
    Latest Posts
  </h2>

  <div style="
    height:1px;
    flex:1;
    margin-left:16px;
    background:linear-gradient(90deg, rgba(59,130,246,0.45), rgba(124,58,237,0.35), transparent);
  "></div>
</div>


<div style="height:18px;"></div>


<!-- POSTS GRID (unchanged) -->
<div style="
  display:grid;
  grid-template-columns:repeat(auto-fill, minmax(260px,1fr));
  gap:20px;
  opacity:0;
  animation:postContainer 1.1s ease forwards;
  animation-delay:0.15s;
">
  {% for post in site.posts %}
  <a href="{{ post.url | relative_url }}" style="text-decoration:none; color:inherit;">
    <div style="
      border:1px solid rgba(255,255,255,0.06);
      border-radius:12px;
      padding:20px;
      background:linear-gradient(180deg, rgba(14,18,28,0.55), rgba(8,10,18,0.3));
      backdrop-filter:blur(10px);
      transition:transform .28s ease, box-shadow .28s ease;
      position:relative;
    "
      onmouseover="this.style.transform='translateY(-6px) scale(1.02)'; this.style.boxShadow='0 0 28px rgba(60,115,246,0.22)';"
      onmouseout="this.style.transform='none'; this.style.boxShadow='none';"
    >
      <div style="font-size:.78rem; color:#9ca3af; margin-bottom:6px;">
        {{ post.date | date: "%d %b %Y" }}
      </div>

      <h3 style="
        margin:0 0 8px 0;
        font-size:1.07rem;
        font-weight:600;
      ">
        {{ post.title }}
      </h3>

      <p style="color:#9ca3af; font-size:.92rem; margin:0;">
        {{ post.excerpt | strip_html | truncate: 130 }}
      </p>

      <div style="
        position:absolute;
        bottom:0;
        left:0;
        width:100%;
        height:2px;
        background:linear-gradient(90deg,#3b82f6,#7c3aed);
        opacity:.35;
      "></div>

    </div>
  </a>
  {% endfor %}
</div>


<!-- ANIMATIONS -->
<style>

/* DESCRIPTION CONTAINER ANIMATION (smooth fade + rise) */
@keyframes descContainerAnim {
  0% {
    opacity:0;
    transform:translateY(20px);
    filter:blur(14px);
  }
  70% {
    opacity:1;
    transform:translateY(0);
    filter:blur(0);
  }
  100% { opacity:1; }
}

/* Posts container animation (unchanged) */
@keyframes postContainer {
  0% {
    opacity:0;
    transform:translateY(26px) scale(0.96);
    filter:blur(14px);
  }
  60% {
    opacity:1;
    transform:translateY(0) scale(1.02);
    filter:blur(0);
  }
  100% {
    opacity:1;
    transform:scale(1);
  }
}
</style>
