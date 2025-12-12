---
layout: default
title: Contact
---

<section style="
  box-sizing:border-box;
  margin-top:0;
  border:1px solid rgba(255,255,255,0.04);
  padding:40px;
  border-radius:14px;
  background:linear-gradient(180deg, rgba(11,14,20,0.70), rgba(6,8,12,0.46));
  backdrop-filter:blur(14px);
  position:relative;
  overflow:visible;
  opacity:0;
  animation:contactReveal 0.95s ease forwards;
">

  <!-- Soft glow behind title -->
  <div aria-hidden="true" style="
    position:absolute;
    left:48px;
    top:18px;
    width:320px;
    height:110px;
    pointer-events:none;
    background: radial-gradient(closest-side, rgba(59,130,246,0.08), rgba(124,58,237,0.06), transparent 60%);
    filter: blur(28px);
    border-radius: 50%;
    z-index:0;
  "></div>

  <div style="position:relative; z-index:2; max-width:1200px; margin:0 auto;">
    <h1 style="
      margin:0 0 6px 0;
      font-size:2rem;
      font-weight:700;
      background:linear-gradient(90deg,#3b82f6,#7c3aed);
      -webkit-background-clip:text;
      -webkit-text-fill-color:transparent;
    ">Get in Touch</h1>

    <!-- underline -->
    <div style="
      height:6px;
      width:220px;
      margin-top:12px;
      border-radius:999px;
      background:linear-gradient(90deg, rgba(59,130,246,0.95), rgba(124,58,237,0.95));
      box-shadow: 0 10px 40px rgba(59,130,246,0.12), 0 0 44px rgba(124,58,237,0.08);
      animation:underlineIn .9s ease forwards;
    "></div>

    <p style="
      color:#b3b7c3;
      max-width:760px;
      font-size:1.05rem;
      line-height:1.6;
      margin:16px 0 28px 0;
    ">
      If you'd like to collaborate, share an idea, or ask about something you're building, send a concise note here.
      I read thoughtful messages and reply when it makes sense.
    </p>
  </div>

  <!-- GRID: make form the highlight -->
  <div class="contact-grid" style="
    display:grid;
    grid-template-columns: 1.6fr 1fr; /* form larger, details smaller */
    gap:32px;
    max-width:1200px;
    margin:0 auto;
    align-items:start;
  ">

    <!-- FORM CARD (HIGHLIGHTED) -->
    <div class="card form-card highlight" style="
      opacity:0;
      animation:fadeSlide .95s ease forwards;
      animation-delay:.12s;
      overflow:hidden;
      border:1px solid rgba(255,255,255,0.08);
      box-shadow: 0 28px 80px rgba(2,6,23,0.6), inset 0 1px 0 rgba(255,255,255,0.02);
    ">
      <form id="contactForm" action="https://formspree.io/f/mpwvklre" method="POST" novalidate>

        <div class="field">
          <label for="name">Your name</label>
          <input id="name" name="name" type="text" placeholder=" " required />
        </div>

        <div class="field">
          <label for="email">Email</label>
          <input id="email" name="email" type="email" placeholder=" " required />
        </div>

        <div class="field">
          <label for="message">Message</label>
          <textarea id="message" name="message" rows="6" placeholder=" " required></textarea>
        </div>

        <div style="display:flex; justify-content:center; margin-top:10px;">
          <button id="submitBtn" type="submit" class="primary-btn" aria-live="polite">
            <span>Send message</span>
          </button>
        </div>

        <div id="formStatus" style="text-align:center; margin-top:12px; font-size:.95rem; color:#9ca3af;"></div>

      </form>
    </div>

    <!-- CONTACT DETAILS (de-emphasized, gmail as plain text) -->
    <aside class="card info-card" style="
      opacity:0;
      animation:fadeSlide .95s ease forwards;
      animation-delay:.28s;
      padding:28px 26px;
      position:relative;
      overflow:visible;
      transition: box-shadow .25s ease, transform .25s ease;
      border:1px solid rgba(255,255,255,0.03);
      background: linear-gradient(180deg, rgba(10,12,16,0.45), rgba(8,10,12,0.22));
    ">

      <!-- left gradient accent (subtle) -->
      <div aria-hidden="true" style="
        position:absolute;
        left:0;
        top:0;
        bottom:0;
        width:6px;
        background: linear-gradient(180deg, rgba(59,130,246,0.9), rgba(124,58,237,0.85));
        border-top-left-radius:12px;
        border-bottom-left-radius:12px;
        opacity:0.9;
      "></div>

      <div style="margin-left:16px;">
        <div style="color:#d6d9e0; font-weight:800; font-size:1.05rem; margin-bottom:12px;">
          Contact Details
        </div>

        <div style="display:flex; flex-direction:column; gap:16px;">

          <div>
            <div style="font-size:.82rem; color:#8c92a0; letter-spacing:.05em; font-weight:600; margin-bottom:6px;">Email</div>
            <!-- plain text (no link) -->
            <div style="color:#cfd3dd; font-weight:700; font-size:.98rem; line-height:1.4;">shanikashameem7@gmail.com</div>
          </div>

          <div>
            <div style="font-size:.82rem; color:#8c92a0; letter-spacing:.05em; font-weight:600; margin-bottom:6px;">LinkedIn</div>
            <a class="contact-link" href="https://www.linkedin.com/in/shanikashameems" target="_blank">
              linkedin.com/in/shanikashameems
            </a>
          </div>

          <div>
            <div style="font-size:.82rem; color:#8c92a0; letter-spacing:.05em; font-weight:600; margin-bottom:6px;">GitHub</div>
            <a class="contact-link" href="https://github.com/shanikashameems" target="_blank">
              github.com/shanikashameems
            </a>
          </div>

          <div style="color:#8c92a0; font-size:.92rem; line-height:1.55; margin-top:6px;">
            I reply to well-structured collaboration requests and scoped project ideas.
          </div>

        </div>
      </div>
    </aside>

  </div> <!-- /grid -->

  <!-- small closing line to fill gap before footer -->
  <div style="max-width:1200px; margin:28px auto 6px; text-align:center; color:#9ca3af; font-size:.95rem;">
    Thanks for visiting — if this looks interesting, say hello. I read everything meaningful.
  </div>

</section>

<!-- SUCCESS MODAL -->
<div id="sentModal" style="
  position:fixed;
  left:50%;
  top:20%;
  transform:translate(-50%,-25%);
  min-width:280px;
  max-width:90%;
  background:linear-gradient(180deg, rgba(17,21,30,0.98), rgba(12,14,18,0.98));
  border:1px solid rgba(255,255,255,0.08);
  padding:18px 20px;
  border-radius:12px;
  box-shadow:0 30px 60px rgba(0,0,0,0.6);
  display:flex;
  gap:12px;
  align-items:center;
  opacity:0;
  pointer-events:none;
  z-index:9999;
">
  <div style="flex:0 0 46px; height:46px; border-radius:10px; background:linear-gradient(90deg,#3b82f6,#7c3aed); display:grid; place-items:center;">
    <svg width="22" height="22" fill="none"><path d="M5 13l4 4L19 7" stroke="white" stroke-width="2.2" stroke-linecap="round"/></svg>
  </div>

  <div style="flex:1;">
    <div style="font-weight:700; color:white;">Message sent</div>
    <div style="color:#cbd0d6; margin-top:4px;">Form submitted successfully</div>
  </div>
</div>

<style>
/* layout safety */
* { box-sizing: border-box; }

/* general tokens */
:root{
  --accent-1: #3b82f6;
  --accent-2: #7c3aed;
  --muted: #8c92a0;
  --label-bright: #cfd3dd;
  --input-text: #eef1f6;
}

/* cards */
.card{
  border-radius:12px;
  background:linear-gradient(180deg, rgba(12,14,18,0.48), rgba(6,8,12,0.18));
  padding:20px;
  border:1px solid rgba(255,255,255,0.03);
}

/* Form card highlight tweaks */
.card.form-card.highlight{
  background: linear-gradient(180deg, rgba(18,22,28,0.72), rgba(9,10,14,0.36));
  border:1px solid rgba(255,255,255,0.08);
}

/* fields */
.field{
  margin-bottom:14px;
  display:flex;
  flex-direction:column;
}
.field label{
  font-size:.95rem;
  color:var(--label-bright);
  font-weight:600;
  margin-bottom:8px;
}

.field input,
.field textarea{
  width:100%;
  padding:12px;
  border-radius:10px;
  border:1px solid rgba(255,255,255,0.10);
  background:rgba(0,0,0,0.28);
  color:var(--input-text);
  font-size:.98rem;
  line-height:1.4;
  resize:vertical;
}

/* focus */
.field input:focus,
.field textarea:focus{
  transform:translateY(-1px);
  border-color:rgba(255,255,255,0.18);
  box-shadow:
    0 20px 50px rgba(59,130,246,0.08),
    0 0 44px rgba(124,58,237,0.05);
}

/* label uplift */
.field.filled label,
.field:focus-within label{
  transform:translateY(-6px);
  color:var(--accent-1);
}

/* small button (Option A) */
.primary-btn{
  padding:8px 16px;
  border-radius:8px;
  background:linear-gradient(90deg,var(--accent-1),var(--accent-2));
  border:none;
  color:white;
  font-weight:700;
  cursor:pointer;
  transition:transform .15s, box-shadow .18s;
  box-shadow:0 8px 28px rgba(59,130,246,0.12);
}
.primary-btn:hover{
  transform:translateY(-3px);
  box-shadow:0 22px 48px rgba(59,130,246,0.16);
}

/* contact links (keep hover only for these) */
.contact-link{
  color:#d3d7e0;
  font-weight:700;
  text-decoration:none;
  font-size:.98rem;
  position:relative;
  transition: color .18s ease;
}
.contact-link:hover{
  color:#a9c6ff;
}
.contact-link::after{
  content:"";
  position:absolute;
  left:0;
  bottom:-3px;
  width:0;
  height:2px;
  background:linear-gradient(90deg,var(--accent-1),var(--accent-2));
  transition:width .28s ease;
  border-radius:10px;
}
.contact-link:hover::after{ width:100%; }

/* info card less prominent */
.info-card { opacity:0.95; }
.info-card .contact-link { color:#d3d7e0; }

/* info card hover mild */
.info-card:hover{
  transform:translateY(-2px);
  box-shadow:0 18px 40px rgba(0,0,0,0.45);
}

/* modal */
#sentModal{ transition:opacity .18s ease, transform .18s ease; }
#sentModal.show{ animation:modalIn .42s ease forwards; opacity:1; pointer-events:auto; transform:translate(-50%,0); }

@keyframes modalIn { 0% { opacity:0; transform:translate(-50%,-35%) scale(.96); } 100% { opacity:1; transform:translate(-50%,0) scale(1); } }

/* page animations */
@keyframes underlineIn{ from{transform:scaleX(0);} to{transform:scaleX(1);} }
@keyframes contactReveal{ from{opacity:0; transform:translateY(18px);} to{opacity:1; transform:translateY(0);} }
@keyframes fadeSlide{ from{opacity:0; transform:translateY(14px);} to{opacity:1; transform:translateY(0);} }

/* responsive */
@media (max-width:980px){
  .contact-grid{ grid-template-columns: 1fr; padding:0 16px; }
  .card.form-card.highlight{ box-shadow:0 14px 40px rgba(2,6,23,0.5); }
  .info-card{ margin-top:8px; }
}
</style>

<script>
(function(){

  /* floating label helper */
  document.querySelectorAll('.field').forEach(f => {
    const input = f.querySelector('input, textarea');
    if(!input) return;
    const update = () => {
      if(input.value && input.value.trim() !== "") f.classList.add("filled");
      else f.classList.remove("filled");
    };
    input.addEventListener("input", update);
    input.addEventListener("blur", update);
    update();
  });

  /* form submission */
  const form = document.getElementById('contactForm');
  const status = document.getElementById('formStatus');
  const modal = document.getElementById('sentModal');
  const submitBtn = document.getElementById('submitBtn');

  form.addEventListener('submit', async (e)=>{
    e.preventDefault();
    submitBtn.disabled = true;

    const data = new FormData(form);
    try{
      const res = await fetch(form.action, {
        method:'POST',
        body:data,
        headers:{'Accept':'application/json'}
      });

      if(res.ok){
        form.reset();
        document.querySelectorAll('.field').forEach(f=>f.classList.remove('filled'));

        status.style.color = '#7ee787';
        status.textContent = 'Form submitted successfully';

        modal.classList.add('show');

        // hide after 2 seconds
        setTimeout(()=>{
          modal.classList.remove('show');
          status.textContent = '';
        }, 2000);

      } else {
        status.style.color = '#ff9b9b';
        status.textContent = 'Could not send message';
        setTimeout(()=> status.textContent = '', 2000);
      }
    }catch(err){
      status.style.color = '#ff9b9b';
      status.textContent = 'Could not send message';
      setTimeout(()=> status.textContent = '', 2000);
    } finally {
      submitBtn.disabled = false;
    }
  });

})();
</script>
