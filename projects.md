---
layout: default
title: Projects
---

<section style="
  margin-top:0;
  border:1px solid rgba(255,255,255,0.05);
  padding:38px;
  border-radius:14px;
  background:linear-gradient(180deg, rgba(13,17,28,0.55), rgba(6,8,14,0.35));
  backdrop-filter:blur(12px);
  opacity:0;
  animation:projectsReveal 1s ease forwards;
">

  <h1 style="
    margin:0 0 16px 0;
    font-size:2rem;
    font-weight:700;
    letter-spacing:-0.02em;
    background:linear-gradient(90deg,#3b82f6,#7c3aed);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
  ">
    Projects & Work
  </h1>

  <p style="
    color:#9ca3af;
    font-size:1.05rem;
    max-width:760px;
    line-height:1.6;
    margin:0 0 28px 0;
  ">
    Selected projects and prototypes that reflect a focus on dependable engineering, clear problem-solving, and practical experimentation. Each entry is a concise snapshot — the problem, the approach, and the outcome.
  </p>


  <!-- AI & ML -->
  <div style="opacity:0; animation:fadeSlide 1.05s ease forwards; animation-delay:0.18s;">
    <h2 style="font-size:1.25rem; margin-bottom:10px; font-weight:600;">AI & Machine Learning</h2>

    <div style="color:#9ca3af; line-height:1.6; font-size:1.03rem; max-width:820px;">
      <strong>Diabetes Prediction System</strong><br>
      ML pipeline built to predict diabetes risk from clinical features. Built multiple baseline models, iterated on feature engineering, and evaluated through explainability metrics to improve trust and clarity.

      <div style="height:10px;"></div>

      <strong>Recommendation Prototype</strong><br>
      A lightweight recommendation engine for grocery suggestions that combines collaborative filtering with content signals. Focused on practical evaluation and simple deployment patterns.
    </div>
  </div>


  <!-- Python Tools -->
  <div style="margin-top:28px; opacity:0; animation:fadeSlide 1.05s ease forwards; animation-delay:0.32s;">
    <h2 style="font-size:1.25rem; margin-bottom:10px; font-weight:600;">Python Tools & Utilities</h2>

    <div style="color:#9ca3af; line-height:1.6; font-size:1.03rem; max-width:820px;">
      <strong>File Morpher</strong><br>
      Small CLI utilities for converting between common file formats and automating routine file workflows.

      <div style="height:10px;"></div>

      <strong>Background Remover</strong><br>
      An image-processing utility that isolates foregrounds for downstream editing and prototyping pipelines.

      <div style="height:10px;"></div>

      <strong>QR Generator</strong><br>
      A compact, dependency-light tool for generating QR codes programmatically, designed for fast integration into scripts and web tools.
    </div>
  </div>


  <!-- Web & Mobile -->
  <div style="margin-top:28px; opacity:0; animation:fadeSlide 1.05s ease forwards; animation-delay:0.46s;">
    <h2 style="font-size:1.25rem; margin-bottom:10px; font-weight:600;">Web & Mobile</h2>

    <div style="color:#9ca3af; line-height:1.6; font-size:1.03rem; max-width:820px;">
      <strong>ByteTree — Learning Platform</strong><br>
      Co-founded a student-first education platform focusing on hands-on programming and approachable AI content. Responsibilities included curriculum design, session delivery, and building course infrastructure.

      <div style="height:10px;"></div>

      <strong>Expo Micro-Journal</strong><br>
      Minimal journaling app built with React Native (Expo). Prioritised a clean UX, local-first data storage and a tiny surface area for fast prototyping.
    </div>
  </div>


  <!-- Future work / CTA -->
  <div style="margin-top:28px; opacity:0; animation:fadeSlide 1.05s ease forwards; animation-delay:0.6s;">
    <h2 style="font-size:1.25rem; margin-bottom:10px; font-weight:600;">Next steps</h2>

    <p style="color:#9ca3af; max-width:760px; font-size:1.03rem; line-height:1.6;">
      I’ll publish deeper write-ups and reproducible notebooks for selected projects. If you’re interested in collaboration or want access to a project repo, reach out via my GitHub profile.
    </p>
  </div>

</section>

<!-- ANIMATIONS -->
<style>
@keyframes projectsReveal {
  0% { opacity:0; transform:translateY(18px); filter:blur(12px); }
  70% { opacity:1; transform:translateY(0); filter:blur(0); }
  100% { opacity:1; }
}

@keyframes fadeSlide {
  0% { opacity:0; transform:translateY(14px); filter:blur(10px); }
  70% { opacity:1; transform:translateY(0); filter:blur(0); }
  100% { opacity:1; }
}
</style>
