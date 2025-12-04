---
layout: default
title: Home
---

<!-- TECH HEADER -->
<div style="
  border:1px solid rgba(255,255,255,0.06);
  background: linear-gradient(180deg, rgba(13,17,28,0.55), rgba(6,8,14,0.35));
  padding:32px;
  border-radius:12px;
  backdrop-filter: blur(10px);
  margin-bottom:32px;
">
  <div style="
    display:flex;
    align-items:center;
    gap:10px;
    margin-bottom:16px;
  ">
    <div style="
      width:8px;
      height:8px;
      border-radius:50%;
      background:linear-gradient(90deg,#3b82f6,#7c3aed);
      box-shadow:0 0 12px rgba(60,115,246,0.8);
    "></div>

    <span style="
      font-size:.85rem;
      letter-spacing:1px;
      color:#9ca3af;
      text-transform:uppercase;
    ">
      Developer Journal
    </span>
  </div>

  <h1 style="
    margin:0;
    font-size:1.9rem;
    line-height:1.2;
    font-weight:700;
    letter-spacing:-0.01em;
  ">
    I build projects, explore AI, and document my engineering journey.
  </h1>

  <p style="
    margin-top:10px;
    color:#9ca3af;
    max-width:650px;
    font-size:1rem;
  ">
    Short technical notes, engineering experiments, and project breakdowns —
    written with clarity, precision, and a focus on learning in public.
  </p>
</div>


<!-- SECTION TITLE -->
<div style="
  display:flex;
  align-items:center;
  justify-content:space-between;
  margin-bottom:14px;
">
  <h2 style="margin:0; font-size:1.2rem;">Recent Posts</h2>
  <div style="height:1px; flex:1; margin-left:14px; background:rgba(255,255,255,0.08);"></div>
</div>


<!-- POSTS GRID (TECH STYLE) -->
<div style="
  display:grid;
  grid-template-columns: repeat(auto-fill, minmax(260px,1fr));
  gap:20px;
">
  {% for post in site.posts %}
  <a href="{{ post.url | relative_url }}" style="
    text-decoration:none;
    color:inherit;
  ">
    <div style="
      border:1px solid rgba(255,255,255,0.05);
      padding:20px;
      border-radius:10px;
      background:linear-gradient(180deg, rgba(14,18,28,0.6), rgba(10,13,22,0.35));
      backdrop-filter: blur(6px);
      transition:0.25s ease;
      position:relative;
      overflow:hidden;
    "
    onmouseover="this.style.transform='translateY(-4px)'; this.style.boxShadow='0 0 32px rgba(60,115,246,0.22)';"
    onmouseout="this.style.transform='none'; this.style.boxShadow='none';"
    >
      <div style="font-size:.78rem; color:#9ca3af; margin-bottom:6px;">
        {{ post.date | date: "%d %b %Y" }}
      </div>

      <h3 style="margin:0 0 8px 0; font-size:1.05rem; font-weight:600;">
        {{ post.title }}
      </h3>

      <p style="margin:0; color:#9ca3af; font-size:.9rem;">
        {{ post.excerpt | strip_html | truncate: 120 }}
      </p>

      <!-- glowing bottom border -->
      <div style="
        position:absolute;
        bottom:0;
        left:0;
        width:100%;
        height:2px;
        background:linear-gradient(90deg,#3b82f6,#7c3aed);
        opacity:.45;
      "></div>
    </div>
  </a>
  {% endfor %}
</div>

