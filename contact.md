---
layout: default
title: Contact
---

<section style="
  margin-top:0;
  border:1px solid rgba(255,255,255,0.05);
  padding:38px;
  border-radius:14px;
  background:linear-gradient(180deg, rgba(13,17,28,0.55), rgba(6,8,14,0.35));
  backdrop-filter:blur(12px);
  opacity:0;
  animation:contactReveal 1s ease forwards;
">

  <!-- HEADER -->
  <h1 style="
    margin:0 0 16px 0;
    font-size:2rem;
    font-weight:700;
    letter-spacing:-0.02em;
    background:linear-gradient(90deg,#3b82f6,#7c3aed);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
  ">
    Get in Touch
  </h1>

  <p style="
    color:#9ca3af;
    max-width:760px;
    font-size:1.1rem;
    line-height:1.6;
    margin:0 0 28px 0;
  ">
    If you’re interested in collaborating, discussing ideas, or want to reach out about something I’ve built or written, here’s where you can connect with me.  
    I try to reply to messages that are meaningful, thoughtful, and aligned with what I’m working on.
  </p>


  <!-- CONTACT BLOCK -->
  <div style="
    opacity:0;
    animation:fadeSlide 1.05s ease forwards;
    animation-delay:0.2s;
  ">

    <!-- Email -->
    <div style="
      margin-bottom:22px;
      border:1px solid rgba(255,255,255,0.05);
      padding:18px 20px;
      border-radius:10px;
      background:rgba(15,18,28,0.45);
      backdrop-filter:blur(10px);
      transition:all .25s ease;
    " onmouseover="this.style.transform='translateY(-4px)'; this.style.borderColor='rgba(59,130,246,0.55)'; this.style.boxShadow='0 0 20px rgba(59,130,246,0.25)';"
      onmouseout="this.style.transform='none'; this.style.borderColor='rgba(255,255,255,0.05)'; this.style.boxShadow='none';"
    >
      <div style="color:#e5e7eb; font-size:1.05rem; font-weight:600;">Email</div>
      <div style="color:#9ca3af; font-size:.97rem; margin-top:4px;">
        shanikashameem7@gmail.com
      </div>
    </div>

    <!-- LinkedIn -->
    <a href="https://www.linkedin.com/in/shanikashameems" target="_blank" style="text-decoration:none; color:inherit;">
      <div style="
        margin-bottom:22px;
        border:1px solid rgba(255,255,255,0.05);
        padding:18px 20px;
        border-radius:10px;
        background:rgba(15,18,28,0.45);
        backdrop-filter:blur(10px);
        transition:all .25s ease;
      " onmouseover="this.style.transform='translateY(-4px)'; this.style.borderColor='rgba(124,58,237,0.55)'; this.style.boxShadow='0 0 20px rgba(124,58,237,0.25)';"
        onmouseout="this.style.transform='none'; this.style.borderColor='rgba(255,255,255,0.05)'; this.style.boxShadow='none';"
      >
        <div style="color:#e5e7eb; font-size:1.05rem; font-weight:600;">LinkedIn</div>
        <div style="color:#9ca3af; font-size:.97rem; margin-top:4px;">
          linkedin.com/in/shanikashameems
        </div>
      </div>
    </a>

    <!-- GitHub -->
    <a href="https://github.com/shanikashameems" target="_blank" style="text-decoration:none; color:inherit;">
      <div style="
        margin-bottom:22px;
        border:1px solid rgba(255,255,255,0.05);
        padding:18px 20px;
        border-radius:10px;
        background:rgba(15,18,28,0.45);
        backdrop-filter:blur(10px);
        transition:all .25s ease;
      " onmouseover="this.style.transform='translateY(-4px)'; this.style.borderColor='rgba(59,130,246,0.55)'; this.style.boxShadow='0 0 20px rgba(59,130,246,0.25)';"
        onmouseout="this.style.transform='none'; this.style.borderColor='rgba(255,255,255,0.05)'; this.style.boxShadow='none';"
      >
        <div style="color:#e5e7eb; font-size:1.05rem; font-weight:600;">GitHub</div>
        <div style="color:#9ca3af; font-size:.97rem; margin-top:4px;">
          github.com/shanikashameems
        </div>
      </div>
    </a>

  </div>

</section>

<!-- ANIMATIONS -->
<style>
@keyframes contactReveal {
  0% { opacity:0; transform:translateY(20px); filter:blur(12px); }
  70% { opacity:1; transform:translateY(0); filter:blur(0); }
  100% { opacity:1; }
}

@keyframes fadeSlide {
  0% { opacity:0; transform:translateY(14px); filter:blur(10px); }
  70% { opacity:1; transform:translateY(0); filter:blur(0); }
  100% { opacity:1; }
}
</style>
