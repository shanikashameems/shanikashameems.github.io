---
layout: default
title: Contact
---

<section style="
  box-sizing:border-box;
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

  <!-- Soft glow behind title -->
  <div aria-hidden="true" style="
    position:absolute;
    left:48px;
    top:18px;
    width:320px;
    height:110px;
    pointer-events:none;
    background: radial-gradient(closest-side, rgba(59,130,246,0.07), rgba(124,58,237,0.05), transparent 60%);
    filter: blur(28px);
    border-radius: 50%;
    z-index:0;
  "></div>

  <div style="position:relative; z-index:2; max-width:1100px; margin:0 auto;">
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
      box-shadow: 0 8px 30px rgba(59,130,246,0.12), 0 0 36px rgba(124,58,237,0.08);
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

  <!-- GRID -->
  <div class="contact-grid" style="display:grid; grid-template-columns: 1fr minmax(300px,380px); gap:28px; max-width:1100px; margin:0 auto;">

    <!-- FORM CARD -->
    <div class="card form-card" style="opacity:0; animation:fadeSlide .95s ease forwards; animation-delay:.12s; overflow:hidden;">
      <form id="contactForm" action="https://formspree.io/f/mpwvklre" method="POST">

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
          <button id="submitBtn" type="submit" class="primary-btn">
            <span>Send message</span>
          </button>
        </div>

        <div id="formStatus" style="text-align:center; margin-top:10px; font-size:.95rem; color:#9ca3af;"></div>

      </form>
    </div>

    <!-- CONTACT DETAILS -->
    <aside class="card info-card" style="
      opacity:0;
      animation:fadeSlide .95s ease forwards;
      animation-delay:.28s;
      padding:28px 26px;
      position:relative;
      overflow:hidden;
      transition: box-shadow .25s ease, transform .25s ease;
    ">

      <!-- left gradient accent -->
      <div aria-hidden="true" style="
        position:absolute;
        left:0;
        top:0;
        bottom:0;
        width:6px;
        background: linear-gradient(180deg, #3b82f6, #7c3aed);
        border-top-left-radius:12px;
        border-bottom-left-radius:12px;
      "></div>

      <div style="margin-left:16px;">
        <div style="color:#d6d9e0; font-weight:800; font-size:1.1rem; margin-bottom:14px;">
          Contact Details
        </div>

        <div style="display:flex; flex-direction:column; gap:18px;">

          <div>
            <div style="font-size:.82rem; color:#8c92a0; letter-spacing:.05em; font-weight:600; margin-bottom:4px;">Email</div>
            <a class="contact-link" href="mailto:shanikashameem7@gmail.com">shanikashameem7@gmail.com</a>
          </div>

          <div>
            <div style="font-size:.82rem; color:#8c92a0; letter-spacing:.05em; font-weight:600; margin-bottom:4px;">LinkedIn</div>
            <a class="contact-link" href="https://www.linkedin.com/in/shanikashameems" target="_blank">
              linkedin.com/in/shanikashameems
            </a>
          </div>

          <div>
            <div style="font-size:.82rem; color:#8c92a0; letter-spacing:.05em; font-weight:600; margin-bottom:4px;">GitHub</div>
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
/* GLOBAL */
* { box-sizing:border-box; }

/* Brightened form labels */
.field label{
  font-size:.95rem;
  color:#cfd3dd;
  font-weight:600;
  margin-bottom:8px;
}

/* Brighter input text */
.field input,
.field textarea{
  width:100%;
  padding:12px;
  border-radius:10px;
  border:1px solid rgba(255,255,255,0.12);
  background:rgba(0,0,0,0.26);
  color:#eef1f6;
  font-size:.98rem;
}

/* Accent uplift on focus */
.field input:focus,
.field textarea:focus{
  transform:translateY(-1px);
  border-color:rgba(255,255,255,0.2);
  box-shadow:0 12px 32px rgba(59,130,246,0.08);
}

.field.filled label,
.field:focus-within label{
  transform:translateY(-6px);
  color:#3b82f6;
}

/* BUTTON (Option A size) */
.primary-btn{
  padding:8px 16px;
  border-radius:8px;
  background:linear-gradient(90deg,#3b82f6,#7c3aed);
  border:none;
  color:white;
  font-weight:700;
  cursor:pointer;
  transition:transform .15s, box-shadow .2s;
  box-shadow:0 6px 20px rgba(59,130,246,0.12);
}
.primary-btn:hover{
  transform:translateY(-3px);
  box-shadow:0 16px 30px rgba(59,130,246,0.18);
}

/* CONTACT LINKS — hover effects */
.contact-link{
  color:#d3d7e0;
  font-weight:700;
  text-decoration:none;
  font-size:.98rem;
  position:relative;
  transition:color .2s ease;
}

.contact-link:hover{
  color:#a9c6ff;
}

.contact-link::after{
  content:"";
  position:absolute;
  left:0;
  bottom:-2px;
  width:0;
  height:2px;
  background:linear-gradient(90deg,#3b82f6,#7c3aed);
  transition:width .28s ease;
  border-radius:10px;
}

.contact-link:hover::after{
  width:100%;
}

/* Contact card hover glow */
.info-card:hover{
  transform:translateY(-3px);
  box-shadow:0 18px 38px rgba(0,0,0,0.35);
}

/* MODAL */
#sentModal.show{
  animation:modalIn .4s ease forwards;
  opacity:1;
  pointer-events:auto;
}

@keyframes modalIn{
  0% { opacity:0; transform:translate(-50%,-35%) scale(.9); }
  100% { opacity:1; transform:translate(-50%,0) scale(1); }
}

/* PAGE ANIMATIONS */
@keyframes underlineIn{
  from{transform:scaleX(0);}
  to{transform:scaleX(1);}
}

@keyframes contactReveal{
  from{opacity:0; transform:translateY(18px);}
  to{opacity:1; transform:translateY(0);}
}

@keyframes fadeSlide{
  from{opacity:0; transform:translateY(14px);}
  to{opacity:1; transform:translateY(0);}
}
</style>

<script>
(function(){

  /* Floating label logic */
  document.querySelectorAll('.field').forEach(f => {
    const input = f.querySelector('input, textarea');
    if(!input) return;
    const update = () => {
      if(input.value.trim() !== "") f.classList.add("filled");
      else f.classList.remove("filled");
    };
    input.addEventListener("input", update);
    update();
  });

  /* Form submission */
  const form = document.getElementById('contactForm');
  const status = document.getElementById('formStatus');
  const modal = document.getElementById('sentModal');

  form.addEventListener('submit', async (e)=>{
    e.preventDefault();
    const data = new FormData(form);

    try{
      const res = await fetch(form.action,{
        method:'POST',
        body:data,
        headers:{'Accept':'application/json'}
      });

      if(res.ok){
        form.reset();
        status.style.color="#7ee787";
        status.textContent="Form submitted successfully";

        modal.classList.add("show");

        setTimeout(()=>{
          modal.classList.remove("show");
          status.textContent="";
        },2000);
      }
    }catch(err){
      status.style.color="#ff9b9b";
      status.textContent="Could not send message";
      setTimeout(()=>status.textContent="",2000);
    }
  });

})();
</script>
