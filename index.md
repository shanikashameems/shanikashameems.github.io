---
layout: default
title: Home
---

<!-- INTRO / HERO -->
<section style="
  border:1px solid rgba(255,255,255,0.05);
  padding:38px;
  border-radius:14px;
  background:linear-gradient(180deg, rgba(13,17,28,0.55), rgba(6,8,14,0.32));
  backdrop-filter:blur(12px);
  animation:fadeIn 1s ease forwards;
  opacity:0;
">
  <div style="
    font-size:.8rem;
    text-transform:uppercase;
    letter-spacing:2px;
    margin-bottom:12px;
    background:linear-gradient(90deg,#3b82f6,#7c3aed);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
    font-weight:600;
  ">
    Shanika's Engineering Notebook
  </div>

  <h1 style="
    margin:0 0 10px 0;
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


<!-- LESS SPACE ABOVE POSTS: MOVED UP -->
<div style="height:24px;"></div>


<!-- POSTS HEADER -->
<div style="
  display:flex;
  align-items:center;
  justify-content:space-between;
  animation:fadeIn 1.2s ease forwards;
  opacity:0;
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


<!-- POSTS GRID -->
<div style="
  display:grid;
  grid-template-columns:repeat(auto-fill, minmax(260px,1fr));
  gap:20px;
">
  {% for post in site.posts %}
  <a href="{{ post.url | relative_url }}" style="text-decoration:none; color:inherit;">

    <div style="
      border:1px solid rgba(255,255,255,0.06);
      border-radius:12px;
      padding:20px;
      background:linear-gradient(180deg, rgba(14,18,28,0.55), rgba(8,10,18,0.3));
      backdrop-filter:blur(10px);
      transition:transform .28s cubic-bezier(.2,.9,.3,1), box-shadow .28s ease;
      opacity:0;
      animation:fadeUp 0.7s ease forwards;
      animation-delay:{{ forloop.index | times: 0.08 }}s;
      position:relative;
    "
      onmouseover="this.style.transform='translateY(-6px)'; this.style.boxShadow='0 0 28px rgba(60,115,246,0.22)';"
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
@keyframes fadeIn {
  from { opacity:0; transform:translateY(8px); filter:blur(15px); }
  to   { opacity:1; transform:none; filter:blur(0); }
}

@keyframes fadeUp {
  from { opacity:0; transform:translateY(22px); filter:blur(10px); }
  to   { opacity:1; transform:none; filter:blur(0); }
}

main {
  animation:pageReveal 0.9s ease-out;
}
@keyframes pageReveal {
  0%   { opacity:0; filter:blur(20px); transform:translateY(28px); }
  70%  { opacity:1; filter:blur(0); transform:translateY(0); }
  100% { opacity:1; }
}
</style>
