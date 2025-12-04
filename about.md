---
layout: default
title: About Me
---

<section style="
  margin-top:0;
  border:1px solid rgba(255,255,255,0.05);
  padding:38px;
  border-radius:14px;
  background:linear-gradient(180deg, rgba(13,17,28,0.55), rgba(6,8,14,0.35));
  backdrop-filter:blur(12px);
  opacity:0;
  animation:aboutReveal 1s ease forwards;
">

  <!-- ABOUT TITLE -->
  <h1 style="
    margin:0 0 16px 0;
    font-size:2rem;
    font-weight:700;
    letter-spacing:-0.02em;
    background:linear-gradient(90deg,#3b82f6,#7c3aed);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
  ">
    About Me
  </h1>

  <!-- SUBTITLE -->
  <p style="
    color:#9ca3af;
    font-size:1.15rem;
    max-width:720px;
    line-height:1.55;
    margin:0 0 28px 0;
  ">
    I’m Shanika, a developer who loves building things that challenge my understanding of how systems work and how intelligence can be engineered. My work sits at the intersection of software, machine learning, and the curiosity to break down complex ideas into elegant, functional solutions.
  </p>

  <!-- SECTION BLOCK -->
  <div style="
    opacity:0;
    animation:fadeSlide 1.1s ease forwards;
    animation-delay:0.25s;
  ">
    <h2 style="
      font-size:1.3rem;
      margin-bottom:10px;
      font-weight:600;
    ">
      What I'm Currently Exploring
    </h2>

    <ul style="
      color:#9ca3af;
      line-height:1.6;
      font-size:1.05rem;
      margin-left:18px;
    ">
      <li>AI and machine learning systems that go beyond basic predictions</li>
      <li>Developing products that combine engineering clarity and design sense</li>
      <li>Teaching through ByteTree — simplifying difficult concepts into practical lessons</li>
      <li>Understanding how software teams scale ideas from scratch to production</li>
    </ul>
  </div>

  <!-- SECTION BLOCK 2 -->
  <div style="
    margin-top:34px;
    opacity:0;
    animation:fadeSlide 1.1s ease forwards;
    animation-delay:0.45s;
  ">
    <h2 style="
      font-size:1.3rem;
      margin-bottom:10px;
      font-weight:600;
    ">
      A Glimpse of My Journey
    </h2>

    <p style="
      color:#9ca3af;
      max-width:760px;
      font-size:1.05rem;
      line-height:1.6;
    ">
      I co-founded ByteTree, a student-run learning platform focused on building solid foundations in programming and AI. 
      Along the way, I explored machine learning models, web engineering, app development, and data science through internships and personal projects.
      Every project I build is an attempt to understand a concept more deeply and create something meaningful out of it.
    </p>
  </div>

  <!-- SECTION BLOCK 3 -->
  <div style="
    margin-top:34px;
    opacity:0;
    animation:fadeSlide 1.1s ease forwards;
    animation-delay:0.65s;
  ">
    <h2 style="
      font-size:1.3rem;
      margin-bottom:10px;
      font-weight:600;
    ">
      What This Space Means to Me
    </h2>

    <p style="
      color:#9ca3af;
      max-width:760px;
      font-size:1.05rem;
      line-height:1.6;
    ">
      This site is my engineering notebook — a place where I document experiments, ideas, challenges, and the small breakthroughs that keep me moving forward.
      It’s less about perfection and more about growth. I learn something new every day, and this space is where those learnings take shape.
    </p>
  </div>

</section>

<!-- ANIMATIONS -->
<style>
@keyframes aboutReveal {
  0% { opacity:0; transform:translateY(20px); filter:blur(12px);}
  70% { opacity:1; transform:translateY(0); filter:blur(0);}
  100% { opacity:1; }
}

@keyframes fadeSlide {
  0% { opacity:0; transform:translateY(18px); filter:blur(10px);}
  70% { opacity:1; transform:translateY(0px); filter:blur(0);}
  100% { opacity:1; }
}
</style>
