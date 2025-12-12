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
    margin:0 0 12px 0;
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
    font-size:1.05rem;
    line-height:1.6;
    margin:0 0 26px 0;
  ">
    If you'd like to collaborate, discuss a project, or ask about my work, send me a concise message — I read every thoughtful note and respond when I can.
  </p>

  <!-- CONTACT FORM + INFO -->
  <div style="display:grid; grid-template-columns: 1fr 360px; gap:22px;">

    <!-- FORM CARD -->
    <div style="
      border:1px solid rgba(255,255,255,0.05);
      padding:18px;
      border-radius:12px;
      background:linear-gradient(180deg, rgba(14,18,28,0.55), rgba(10,12,18,0.18));
      backdrop-filter:blur(8px);
      opacity:0;
      animation:fadeSlide 1s ease forwards;
      animation-delay:0.18s;
    ">

      <!--
        IMPORTANT:
        Replace ACTION_URL below with your Formspree endpoint:
        Example: https://formspree.io/f/yourFormId
      -->
      <form id="contactForm"
            action="https://formspree.io/f/ACTION_URL" method="POST">

        <label style="display:block; font-size:.92rem; color:#e5e7eb; margin-bottom:8px; font-weight:600;">
          Your name
        </label>
        <input name="name" required
               style="width:100%; padding:10px 12px; border-radius:8px; border:1px solid rgba(255,255,255,0.04); background:rgba(0,0,0,0.2); color:var(--text); outline:none; margin-bottom:12px;" />

        <label style="display:block; font-size:.92rem; color:#e5e7eb; margin-bottom:8px; font-weight:600;">
          Email
        </label>
        <input name="email" type="email" required
               style="width:100%; padding:10px 12px; border-radius:8px; border:1px solid rgba(255,255,255,0.04); background:rgba(0,0,0,0.2); color:var(--text); outline:none; margin-bottom:12px;" />

        <label style="display:block; font-size:.92rem; color:#e5e7eb; margin-bottom:8px; font-weight:600;">
          Message
        </label>
        <textarea name="message" rows="6" required
               style="width:100%; padding:10px 12px; border-radius:8px; border:1px solid rgba(255,255,255,0.04); background:rgba(0,0,0,0.2); color:var(--text); outline:none; margin-bottom:12px;"></textarea>

        <div style="display:flex; gap:12px; align-items:center;">
          <button type="submit"
            style="padding:10px 14px; border-radius:10px; background:linear-gradient(90deg,#3b82f6,#7c3aed); border:none; color:white; font-weight:700; cursor:pointer;">
            Send message
          </button>

          <div id="formStatus" style="color:#9ca3af; font-size:.95rem;"></div>
        </div>
      </form>

      <!-- JS: AJAX submit for nicer UX (also falls back to form action without JS) -->
      <script>
      (function () {
        const form = document.getElementById('contactForm');
        const status = document.getElementById('formStatus');

        form.addEventListener('submit', async function (e) {
          e.preventDefault();
          status.textContent = 'Sending...';

          const action = form.getAttribute('action');
          const data = new FormData(form);

          try {
            const res = await fetch(action, {
              method: 'POST',
              headers: {
                'Accept': 'application/json'
              },
              body: data
            });

            if (res.ok) {
              form.reset();
              status.style.color = '#7ee787';
              status.textContent = 'Message sent — I will get back to you.';
            } else {
              const json = await res.json().catch(()=>{});
              status.style.color = '#ff9b9b';
              status.textContent = (json && json.error) ? json.error : 'Could not send — try again later.';
            }
          } catch (err) {
            status.style.color = '#ff9b9b';
            status.textContent = 'Network error — check your endpoint and try again.';
          }

          // subtle reset of status color after 5s
          setTimeout(() => {
            status.style.color = '#9ca3af';
          }, 5000);
        });
      })();
      </script>
    </div>

    <!-- INFO CARD -->
    <div style="
      border:1px solid rgba(255,255,255,0.05);
      padding:18px;
      border-radius:12px;
      background:rgba(15,18,28,0.45);
      backdrop-filter:blur(8px);
      display:flex;
      flex-direction:column;
      gap:12px;
      opacity:0;
      animation:fadeSlide 1s ease forwards;
      animation-delay:0.32s;
    ">

      <div style="color:#e5e7eb; font-weight:700; font-size:1.02rem;">Contact</div>
      <div style="color:#9ca3af; font-size:.95rem;">Email</div>
      <div style="color:#e5e7eb; font-weight:600;">shanikashameem7@gmail.com</div>

      <div style="height:8px;"></div>

      <div style="color:#9ca3af; font-size:.95rem;">LinkedIn</div>
      <a href="https://www.linkedin.com/in/shanikashameems" target="_blank" style="color:#e5e7eb; font-weight:600; text-decoration:none;">
        linkedin.com/in/shanikashameems
      </a>

      <div style="height:8px;"></div>

      <div style="color:#9ca3af; font-size:.95rem;">GitHub</div>
      <a href="https://github.com/shanikashameems" target="_blank" style="color:#e5e7eb; font-weight:600; text-decoration:none;">
        github.com/shanikashameems
      </a>

      <div style="flex:1"></div>

      <div style="font-size:.9rem; color:#9ca3af;">
        I usually reply to focused collaboration requests, reproducible bug reports, and well-scoped ideas. If you’re reaching out about general feedback, a short message is best.
      </div>

    </div>

  </div>

  <!-- FOOTER MESSAGE INSIDE PAGE -->
  <div style="
    margin-top:22px;
    border-top:1px solid rgba(255,255,255,0.03);
    padding-top:18px;
    color:#9ca3af;
    font-size:.98rem;
    opacity:0;
    animation:fadeSlide 1s ease forwards;
    animation-delay:0.5s;
  ">
    Thanks for stopping by — if your message needs a reply, I will respond as soon as I can.
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

/* small responsive fallback */
@media (max-width:880px) {
  .contact-grid { grid-template-columns: 1fr; }
  section > div[style*="display:grid"] { grid-template-columns: 1fr; }
}
</style>
