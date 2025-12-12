---
layout: default
title: Contact
---

<section style="
  margin-top:0;
  border:1px solid rgba(255,255,255,0.06);
  padding:40px;
  border-radius:14px;
  background:linear-gradient(180deg, rgba(13,17,28,0.64), rgba(6,8,14,0.42));
  backdrop-filter:blur(12px);
  position:relative;
  overflow:visible;
  opacity:0;
  animation:contactReveal 0.95s ease forwards;
">

  <!-- Soft background glow behind title (B) -->
  <div aria-hidden="true" style="
    position:absolute;
    left:48px;
    top:18px;
    width:360px;
    height:120px;
    pointer-events:none;
    background: radial-gradient(closest-side, rgba(59,130,246,0.08), rgba(124,58,237,0.06), transparent 60%);
    filter: blur(28px);
    transform: translateZ(0);
    border-radius: 50%;
    z-index:0;
  "></div>

  <div style="position:relative; z-index:2;">
    <h1 style="
      margin:0 0 6px 0;
      font-size:2rem;
      font-weight:700;
      letter-spacing:-0.02em;
      display:inline-block;
      background:linear-gradient(90deg,#3b82f6,#7c3aed);
      -webkit-background-clip:text;
      -webkit-text-fill-color:transparent;
    ">
      Get in Touch
    </h1>

    <!-- Glowing underline (A) -->
    <div style="
      height:6px;
      width:220px;
      margin-top:12px;
      border-radius:999px;
      background:linear-gradient(90deg, rgba(59,130,246,0.95), rgba(124,58,237,0.95));
      box-shadow: 0 8px 30px rgba(59,130,246,0.12), 0 0 36px rgba(124,58,237,0.08);
      opacity:0.95;
      transform-origin:left center;
      animation:underlineIn .9s ease forwards;
    "></div>

    <p style="
      color:#b3b7c3;
      max-width:760px;
      font-size:1.05rem;
      line-height:1.6;
      margin:16px 0 26px 0;
    ">
      If you'd like to collaborate, share an idea, or ask about something you're building, send a concise note here.  
      I read thoughtful messages and reply when it makes sense.
    </p>
  </div>


  <!-- GRID: form + info -->
  <div class="contact-grid" style="display:grid; grid-template-columns:1fr 360px; gap:24px; position:relative; z-index:2;">

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
            <span class="btn-text">Send message</span>
            <span class="btn-loader" aria-hidden="true"></span>
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
    position:relative;
    z-index:2;
  ">
    Thanks for taking the time to reach out — if your message needs a reply, I’ll get back to you soon.
  </div>

</section>

<!-- MESSAGE SENT MODAL -->
<div id="sentModal" role="dialog" aria-modal="true" aria-hidden="true" style="
  position:fixed;
  left:50%;
  top:18%;
  transform:translate(-50%,-20%);
  min-width:280px;
  max-width:90%;
  background:linear-gradient(180deg, rgba(17,21,30,0.98), rgba(12,14,18,0.98));
  border:1px solid rgba(255,255,255,0.06);
  padding:18px 20px;
  border-radius:12px;
  box-shadow: 0 30px 60px rgba(2,6,23,0.7);
  display:flex;
  gap:12px;
  align-items:center;
  z-index:9999;
  opacity:0;
  pointer-events:none;
">
  <div style="flex:0 0 46px; height:46px; border-radius:10px; display:grid; place-items:center; background:linear-gradient(90deg,#3b82f6,#7c3aed); box-shadow:0 8px 30px rgba(59,130,246,0.18);">
    <svg width="22" height="22" viewBox="0 0 24 24" fill="none" aria-hidden="true"><path d="M5 13l4 4L19 7" stroke="white" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/></svg>
  </div>

  <div style="flex:1;">
    <div id="modalTitle" style="font-weight:700; color:#e5e7eb;">Message sent</div>
    <div id="modalText" style="color:#b9bec8; font-size:.95rem; margin-top:6px;">Thanks — I received your message and will reply when I can.</div>
  </div>

  <button id="modalClose" aria-label="Close" style="
    background:transparent; border:none; color:#9ca3af; font-weight:700; cursor:pointer;
  ">Close</button>
</div>

<!-- CONFETTI-LIKE SPARKS (CSS) -->
<style>
/* small entrance for underline */
@keyframes underlineIn {
  0% { transform: scaleX(0); opacity:0; }
  60% { transform: scaleX(1.02); opacity:1; }
  100% { transform: scaleX(1); opacity:1; }
}

/* general card + field styles (improved visuals) */
:root{
  --accent-1: #3b82f6;
  --accent-2: #7c3aed;
  --muted: #9ca3af;
  --bg-input: rgba(0,0,0,0.26);
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

/* labels (above) */
.field label{
  font-size:.95rem;
  color:var(--muted);
  font-weight:600;
  margin-bottom:8px;
  transform-origin:left center;
  transition: transform .22s cubic-bezier(.2,.9,.3,1), color .18s ease, opacity .18s ease;
}

/* inputs */
.field input,
.field textarea{
  width:100%;
  padding:12px;
  border-radius:10px;
  border:1px solid rgba(255,255,255,0.12);
  background:var(--bg-input);
  color:var(--text);
  font-size:.98rem;
  outline:none;
  transition: box-shadow .18s ease, border-color .18s ease, transform .08s ease;
  -webkit-appearance:none;
}

/* subtle lift */
.field input:focus,
.field textarea:focus{ transform: translateY(-1px); }

/* focus glow (gradient blended) */
.field input:focus,
.field textarea:focus{
  border-color: rgba(255,255,255,0.18);
  box-shadow:
    0 14px 40px rgba(59,130,246,0.08),
    0 0 48px rgba(124,58,237,0.05),
    inset 0 0 0 1px rgba(255,255,255,0.02);
}

/* label uplift when focused / filled */
.field:focus-within label,
.field.filled label{
  transform: translateY(-6px) scale(.99);
  color: var(--accent-1);
  opacity:1;
}

/* primary button with micro-animation */
.primary-btn, .primary-btn .btn-text {
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
.primary-btn:hover{ transform: translateY(-3px); box-shadow: 0 18px 40px rgba(59,130,246,0.12); }

/* loader dot inside button */
.primary-btn .btn-loader{
  display:inline-block;
  width:14px;
  height:14px;
  border-radius:999px;
  margin-left:8px;
  vertical-align:middle;
  opacity:0;
  transform:scale(.8);
  transition: opacity .18s ease, transform .18s ease;
}
.primary-btn.loading .btn-loader{
  opacity:1;
  transform:scale(1);
  background: linear-gradient(90deg, rgba(255,255,255,0.95), rgba(255,255,255,0.6));
  box-shadow: 0 6px 18px rgba(59,130,246,0.08);
}

/* modal show/hide */
#sentModal.show{ animation: modalIn .42s cubic-bezier(.2,.9,.28,1) forwards; opacity:1; pointer-events:auto; transform:translate(-50%,0); top:22%; }
@keyframes modalIn {
  0% { opacity:0; transform:translate(-50%,-18%); filter:blur(6px) scale(.98); }
  60% { opacity:1; transform:translate(-50%,2%); filter:blur(0) scale(1.02); }
  100% { transform:translate(-50%,0); opacity:1; filter:blur(0); }
}

/* success sparkle lines (subtle) */
.sent-spark {
  position:absolute; width:6px; height:2px; background:linear-gradient(90deg,var(--accent-1),var(--accent-2));
  border-radius:2px; opacity:.95; transform-origin:center left;
}
.sent-spark.s1{ left:14px; top:-6px; transform: rotate(18deg) translateX(-6px); animation: sparkMove .9s cubic-bezier(.2,.9,.28,1) forwards; }
.sent-spark.s2{ right:18px; top:-4px; transform: rotate(-28deg) translateX(6px); animation: sparkMove .95s cubic-bezier(.2,.9,.28,1) .06s forwards; }
@keyframes sparkMove { from { opacity:0; transform:scale(.6) translateY(-6px); } to { opacity:1; transform:scale(1) translateY(0); } }

/* basic animations */
@keyframes contactReveal { 0% { opacity:0; transform:translateY(18px); filter:blur(12px); } 70% { opacity:1; transform:translateY(0); filter:blur(0); } 100% { opacity:1; } }
@keyframes fadeSlide { 0% { opacity:0; transform:translateY(12px); filter:blur(10px); } 70% { opacity:1; transform:translateY(0); filter:blur(0); } 100% { opacity:1; } }

/* responsive */
@media (max-width:900px){
  .contact-grid { grid-template-columns: 1fr !important; }
  .card { padding:16px; }
  :root { --accent-1: #3b82f6; --accent-2: #7c3aed; }
}
</style>

<!-- INTERACTIVE JAVASCRIPT -->
<script>
(function () {
  // floating label helper
  const fields = document.querySelectorAll('.field');
  fields.forEach(field => {
    const input = field.querySelector('input, textarea');
    if (!input) return;
    const update = () => {
      if (input.value && input.value.trim() !== '') field.classList.add('filled');
      else field.classList.remove('filled');
    };
    update();
    input.addEventListener('input', update);
    input.addEventListener('blur', update);
    input.addEventListener('focus', () => field.classList.add('focused'));
    input.addEventListener('blur', () => field.classList.remove('focused'));
  });

  // form submission & UI
  const form = document.getElementById('contactForm');
  const status = document.getElementById('formStatus');
  const submitBtn = document.getElementById('submitBtn');
  const modal = document.getElementById('sentModal');
  const modalClose = document.getElementById('modalClose');

  form.addEventListener('submit', async (e) => {
    e.preventDefault();
    status.style.color = getComputedStyle(document.documentElement).getPropertyValue('--muted') || '#9ca3af';
    status.textContent = 'Sending...';
    submitBtn.classList.add('loading');
    submitBtn.disabled = true;

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
        document.querySelectorAll('.field').forEach(f => f.classList.remove('filled'));
        status.classList.add('status-success');
        status.textContent = 'Message sent successfully.';

        // show modal with a small sparkle effect
        modal.classList.add('show');
        modal.setAttribute('aria-hidden', 'false');

        // add small decorative sparks inside modal (DOM)
        ['s1','s2'].forEach(cls => {
          const spark = document.createElement('div');
          spark.className = 'sent-spark ' + cls;
          modal.appendChild(spark);
          // remove after animation
          setTimeout(() => spark.remove(), 1200);
        });

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
      submitBtn.classList.remove('loading');
      submitBtn.disabled = false;
      setTimeout(() => { status.textContent = ''; status.classList.remove('status-success'); }, 5000);
    }
  });

  // close modal
  modalClose.addEventListener('click', () => {
    modal.classList.remove('show');
    modal.setAttribute('aria-hidden', 'true');
  });

  // close with Esc
  document.addEventListener('keydown', (e) => { if (e.key === 'Escape') { modal.classList.remove('show'); modal.setAttribute('aria-hidden','true'); } });

})();
</script>
