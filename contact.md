---
permalink: /contact/
layout: default
title: Contact
---

<section class="content-page reveal">
  <div class="eyebrow">A note is always welcome</div>
  <h1>Let's talk.</h1>
  <p>Have a project in mind, want to exchange ideas, or just want to say hello? Leave a little message below, or find me around the internet.</p>

  <div class="contact-layout">
    <form class="journal-form" action="https://formspree.io/f/mpwvklre" method="POST">
      <label for="name">Your name</label>
      <input id="name" name="name" type="text" autocomplete="name" placeholder="How should I address you?" required>

      <label for="email">Email address</label>
      <input id="email" name="email" type="email" autocomplete="email" placeholder="you@example.com" required>

      <label for="message">Your message</label>
      <textarea id="message" name="message" rows="6" placeholder="Write a little note..." required></textarea>

      <button type="submit">Send message <span aria-hidden="true">↗</span></button>
    </form>

    <aside class="contact-aside">
      <div class="eyebrow">Elsewhere on the internet</div>
      <h2>Find me here.</h2>
      <a href="https://instagram.com/shanikashameem" target="_blank" rel="noopener noreferrer"><span>Instagram</span><small>@shanikashameem</small><b>↗</b></a>
      <a href="mailto:shanikashameem7@gmail.com"><span>Email</span><small>shanikashameem7@gmail.com</small><b>↗</b></a>
      <a href="https://www.linkedin.com/in/shanikashameem" target="_blank" rel="noopener noreferrer"><span>LinkedIn</span><small>/in/shanikashameem</small><b>↗</b></a>
      <a href="https://github.com/shanikashameems" target="_blank" rel="noopener noreferrer"><span>GitHub</span><small>@shanikashameems</small><b>↗</b></a>
      <p>Whether it’s a collaboration, an idea, or just a hello, I’d love to hear from you.</p>
    </aside>
  </div>
</section>

<style>
.contact-layout{display:grid;grid-template-columns:minmax(0,1.5fr) minmax(240px,.9fr);gap:42px;margin-top:42px;align-items:start}
.journal-form{padding:28px;background:#fffdf6;border:2px solid #e9dcca;border-radius:18px;box-shadow:5px 6px 0 rgba(185,217,197,.55)}
.journal-form label{display:block;margin:0 0 7px;font:600 1.35rem var(--caveat);letter-spacing:0;text-transform:none;color:var(--muted)}
.journal-form input,.journal-form textarea{display:block;width:100%;margin:0 0 22px;padding:13px 14px;border:2px solid #eadfce;border-radius:10px;background:#fffaf0;color:var(--ink);font:1.15rem var(--hand);outline:none;transition:border-color .2s,box-shadow .2s}
.journal-form input:focus,.journal-form textarea:focus{border-color:var(--accent);box-shadow:0 0 0 3px rgba(155,87,62,.09)}
.journal-form textarea{resize:vertical;min-height:150px}
.journal-form button{border:0;background:var(--ink);color:var(--paper);padding:13px 18px;font:700 1.45rem var(--caveat);letter-spacing:0;text-transform:none;cursor:pointer;border-radius:12px;box-shadow:3px 4px 0 #d7c8b8;transition:background .2s,transform .2s}
.journal-form button:hover{background:var(--accent);transform:translateY(-2px)}
.journal-form button span{margin-left:22px}
.contact-aside{padding:5px 0}
.contact-aside h2{font:400 2.8rem/.95 var(--sketch);margin:12px 0 22px}
.contact-aside>a{display:grid;grid-template-columns:1fr auto;gap:1px 12px;text-decoration:none;padding:13px 0;border-bottom:1px solid var(--line);font:700 1.55rem var(--caveat);transition:transform .2s,color .2s}
.contact-aside>a:hover{transform:translateX(4px);color:var(--coral-dark)}
.contact-aside>a small{grid-column:1;font:1rem var(--hand);color:var(--muted);overflow-wrap:anywhere}
.contact-aside>a b{grid-column:2;grid-row:1/3;align-self:center;color:var(--accent);font-weight:400}
.contact-aside p{font-size:.95rem;line-height:1.8;margin-top:26px}
@media(max-width:760px){.contact-layout{grid-template-columns:1fr;gap:32px}.journal-form{padding:20px}}
</style>
