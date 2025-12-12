---
layout: default
title: Contact
---

<section style="
  margin-top:0;
  border:1px solid rgba(255,255,255,0.06);
  padding:36px;
  border-radius:14px;
  background:linear-gradient(180deg, rgba(13,17,28,0.60), rgba(6,8,14,0.40));
  backdrop-filter:blur(12px);
  opacity:0;
  animation:contactReveal 0.95s ease forwards;
">

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
    color:#b3b7c3;
    max-width:760px;
    font-size:1.05rem;
    line-height:1.6;
    margin:0 0 28px 0;
  ">
    If you'd like to collaborate, share an idea, or ask about something you're building, send a concise note here.  
    I read thoughtful messages and reply when it makes sense.
  </p>


  <!-- GRID: form + info -->
  <div class="contact-grid" style="display:grid; grid-template-columns:1fr 360px; gap:24px;">

    <!-- FORM CARD -->
    <div class="card form-card" style="opacity:0; animation:fadeSlide .95s ease forwards; animation-delay:.12s;">
      <form id="contactForm" action="https://formspree.io/f/mpwvklre" method="POST" novalidate>

        <!-- FIELD: Name -->
        <div class="field">
          <label for="name">Your name</label>
          <input id="name" name="name" type="text" placeholder=" " required autocomplete="name" />
        </div>

        <!-- FIELD: Email -->
        <div class="field">
          <label for="email">Email</label>
          <input id="email" name="email" type="email" placeholder=" " required autocomplete="email" />
        </div>

        <!-- FIELD: Message -->
        <div class="field">
          <label for="message">Message</label>
          <textarea id="message" name="message" rows="6" placeholder=" " required></textarea>
        </div>

        <div style="display:flex; align-items:center; gap:12px; margin-top:6px;">
          <button id="submitBtn" type="submit" class="primary-btn">
            Send message
          </button>

          <div id="formStatus" aria-live="polite" style="color:#9ca3af; font-size:.95rem;"></div>
        </div>
      </form>
    </div>

    <!-- INFO CARD -->
    <aside class="card info-card" style="opacity:0; animation:fadeSlide .95s ease forwards; animation-delay:.28s;">
      <div style="color:#e5e7eb; font-weight:700; font-size:1.03rem;">Contact Details</div>

      <div style="height:10px;"></div>

      <div style="color:#9ca3af; font-size:.95rem;">Email</div>
      <div style="color:#e5e7eb; font-weight:600;">shanikashameem7@gmail.com</div>

      <div style="height:10px;"></div>

      <div style="color:#9ca3af; font-size:.95rem;">LinkedIn</div>
      <a href="https://www.linkedin.com/in/shanikashameems" target="_blank" style="color:#e5e7eb; font-weight:600; text-decoration:none;">
        linkedin.com/in/shanikashameems
      </a>

      <div style="height:10px;"></div>

      <div style="color:#9ca3af; font-size:.95rem;">GitHub</div>
      <a href="https://github.com/shanikashameems" target="_blank" style="color:#e5e7eb; font-weight:600; text-decoration:none;">
        github.com/shanikashameems
      </a>

      <div style="flex:1"></div>

      <div style="font-size:.9rem; color:#9ca3af;">
        I reply to well-structured collaboration requests, technical discussions, and scoped project ideas.
      </div>
    </aside>

  </div> <!-- /grid -->


  <!-- FOOTER TEXT -->
  <div style="
    margin-top:26px;
    border-top:1px solid rgba(255,255,255,0.05);
    padding-top:18px;
    color:#9ca3af;
    font-size:.95rem;
    opacity:0;
    animation:fadeSlide .95s ease forwards;
    animation-delay:.5s;
  ">
    Thanks for taking the time to reach out — if your message needs a reply, I’ll get back to you soon.
  </div>

</section>


<!-- STYLES & ANIMATIONS -->
<style>
:root{
  --accent-1: #3b82f6;
  --accent-2: #7c3aed;
  --muted: #9ca3af;
  --bg-input: rgba(0,0,0,0.25);
  --text: #e5e7eb;
}

/* cards */
.card{
  border:1px solid rgba(255,255,255,0.08);
  padding:20px;
  border-radius:12px;
  background:linear-gradient(180deg, rgba(14,18,28,0.55), rgba(10,12,18,0.22));
  backdrop-filter:blur(8px);
}

/* fields layout */
.field{
  margin-bottom:14px;
  position:relative;
  display:flex;
  flex-direction:column;
}

/* label above input — subtle default */
.field label{
  font-size:.95rem;
  color:var(--muted);
  font-weight:600;
  transform-origin:left center;
  transition: transform .22s cubic-bezier(.2,.9,.28,1), color .18s ease, opacity .18s ease;
  margin-bottom:8px;
  will-change:transform,opacity;
}

/* input + textarea base */
.field input,
.field textarea{
  width:100%;
  padding:12px;
  border-radius:10px;
  border:1px solid rgba(255,255,255,0.14);
  background:var(--bg-input);
  color:var(--text);
  font-size:.98rem;
  outline:none;
  transition: box-shadow .18s ease, border-color .18s ease, transform .08s ease;
  -webkit-appearance:none;
}

/* subtle inner focus lift */
.field input:focus,
.field textarea:focus{
  transform: translateY(-1px);
}

/* focus glow — gradient blend: blue + purple */
.field input:focus,
.field textarea:focus{
  border-color: rgba(255,255,255,0.18);
  box-shadow:
    0 8px 30px rgba(59,130,246,0.10),
    0 0 40px rgba(124,58,237,0.06),
    inset 0 0 0 1px rgba(255,255,255,0.02);
}

/* label lift on focus or when input has a value (not placeholder-shown) */
.field input:focus + label,
.field textarea:focus + label { /* if label placed after input — but we put label before; using :focus-within below */
  transform: translateY(-4px) scale(.99);
  color: var(--accent-1);
  opacity:1;
}

/* we use focus-within on parent to move label upward since label is above input */
.field:focus-within label{
  transform: translateY(-6px) scale(.99);
  color: var(--accent-1);
  opacity:1;
}

/* when field has content (not placeholder shown) — apply uplift (fallback for focus-within) */
.field input:not(:placeholder-shown) ~ label,
.field textarea:not(:placeholder-shown) ~ label {
  transform: translateY(-6px) scale(.99);
  color: var(--accent-1);
  opacity:1;
}

/* BUT our markup places label BEFORE input; to support above rules reliably, we add a small JS helper that toggles a filled class */
.field.filled label{
  transform: translateY(-6px) scale(.99);
  color: var(--accent-1);
  opacity:1;
}

/* primary button */
.primary-btn{
  padding:11px 16px;
  border-radius:10px;
  background: linear-gradient(90deg, var(--accent-1), var(--accent-2));
  border:none;
  color:white;
  font-weight:700;
  cursor:pointer;
  transition: transform .14s ease, box-shadow .18s ease, opacity .12s ease;
  box-shadow: 0 8px 26px rgba(59,130,246,0.08);
}
.primary-btn:hover{
  transform: translateY(-3px);
  box-shadow: 0 18px 40px rgba(59,130,246,0.12);
}

/* subtle success pulse */
@keyframes successPulse {
  0% { transform: scale(1); opacity:1; }
  50% { transform: scale(1.04); opacity:.95; }
  100% { transform: scale(1); opacity:1; }
}

/* status success */
.status-success{
  color:#7ee787 !important;
  animation: successPulse .9s ease;
}

/* basic animations */
@keyframes contactReveal {
  0% { opacity:0; transform:translateY(18px); filter:blur(12px); }
  70% { opacity:1; transform:translateY(0); filter:blur(0); }
  100% { opacity:1; }
}
@keyframes fadeSlide {
  0% { opacity:0; transform:translateY(12px); filter:blur(10px); }
  70% { opacity:1; transform:translateY(0); filter:blur(0); }
  100% { opacity:1; }
}

/* responsive */
@media (max-width:900px){
  .contact-grid { grid-template-columns: 1fr !important; }
  .card { padding:16px; }
  .field label { margin-bottom:6px; }
}
</style>


<!-- INTERACTIVE JAVASCRIPT (keeps floating state and improves UX) -->
<script>
(function () {
  // keep label lifted if input has value (because we placed label before input)
  const fields = document.querySelectorAll('.field');
  fields.forEach(field => {
    const input = field.querySelector('input, textarea');
    if (!input) return;

    // helper to toggle filled class
    const update = () => {
      if (input.value && input.value.trim() !== '') field.classList.add('filled');
      else field.classList.remove('filled');
    };

    // initial state
    update();

    // events
    input.addEventListener('input', update);
    input.addEventListener('blur', update);
    input.addEventListener('focus', () => field.classList.add('focused'));
    input.addEventListener('blur', () => field.classList.remove('focused'));
  });

  // Form submission (AJAX) — uses your Formspree endpoint and shows status
  const form = document.getElementById('contactForm');
  const status = document.getElementById('formStatus');
  const submitBtn = document.getElementById('submitBtn');

  form.addEventListener('submit', async (e) => {
    e.preventDefault();
    status.style.color = getComputedStyle(document.documentElement).getPropertyValue('--muted') || '#9ca3af';
    status.textContent = 'Sending...';
    submitBtn.disabled = true;
    submitBtn.style.opacity = '.85';

    const action = form.getAttribute('action');
    const data = new FormData(form);

    try {
      const res = await fetch(action, {
        method: 'POST',
        headers: { 'Accept': 'application/json' },
        body: data
      });

      if (res.ok) {
        form.reset();
        // reset filled classes
        document.querySelectorAll('.field').forEach(f => f.classList.remove('filled'));
        status.classList.add('status-success');
        status.textContent = 'Message sent successfully.';
      } else {
        let text = 'Message failed to send.';
        try { const json = await res.json(); if (json && json.error) text = json.error; } catch(e){}
        status.classList.remove('status-success');
        status.style.color = '#ff9b9b';
        status.textContent = text;
      }
    } catch (err) {
      status.classList.remove('status-success');
      status.style.color = '#ff9b9b';
      status.textContent = 'Network error — try again.';
    } finally {
      submitBtn.disabled = false;
      submitBtn.style.opacity = '1';
      setTimeout(() => {
        status.textContent = '';
        status.classList.remove('status-success');
      }, 5000);
    }
  });
})();
</script>
