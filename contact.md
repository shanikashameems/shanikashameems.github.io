---
layout: default
title: Contact
---

<section class="content-page reveal">
  <div class="eyebrow">A note is always welcome</div>
  <h1>Let's talk.</h1>
  <p>Have a project in mind, want to exchange ideas, or just want to say hello? Leave a message below. I’d be happy to hear from you.</p>

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
      <a href="mailto:shanikashameem7@gmail.com">Email <span>↗</span></a>
      <a href="https://www.linkedin.com/in/shanikashameems" target="_blank" rel="noopener noreferrer">LinkedIn <span>↗</span></a>
      <a href="https://github.com/shanikashameems" target="_blank" rel="noopener noreferrer">GitHub <span>↗</span></a>
      <p>I usually appreciate a little context in collaboration messages. It makes replying much easier for both of us.</p>
    </aside>
  </div>
</section>

<style>
.contact-layout{display:grid;grid-template-columns:minmax(0,1.5fr) minmax(220px,.8fr);gap:42px;margin-top:42px;align-items:start}
.journal-form{padding:28px;background:rgba(255,253,247,.58);border:1px solid var(--line)}
.journal-form label{display:block;margin:0 0 7px;font:500 .67rem var(--mono);letter-spacing:.09em;text-transform:uppercase;color:var(--muted)}
.journal-form input,.journal-form textarea{display:block;width:100%;margin:0 0 22px;padding:13px 14px;border:1px solid var(--line);border-radius:0;background:rgba(255,255,255,.5);color:var(--ink);font: .92rem var(--sans);outline:none;transition:border-color .2s,box-shadow .2s}
.journal-form input:focus,.journal-form textarea:focus{border-color:var(--accent);box-shadow:0 0 0 3px rgba(155,87,62,.09)}
.journal-form textarea{resize:vertical;min-height:150px}
.journal-form button{border:0;background:var(--ink);color:var(--paper);padding:13px 18px;font:500 .7rem var(--mono);letter-spacing:.08em;text-transform:uppercase;cursor:pointer;transition:background .2s,transform .2s}
.journal-form button:hover{background:var(--accent);transform:translateY(-2px)}
.journal-form button span{margin-left:22px}
.contact-aside{padding:5px 0}
.contact-aside h2{font-size:1.8rem;margin:12px 0 22px}
.contact-aside>a{display:flex;justify-content:space-between;text-decoration:none;padding:13px 0;border-bottom:1px solid var(--line);font:500 1rem var(--serif)}
.contact-aside>a span{color:var(--accent)}
.contact-aside p{font-size:.86rem;line-height:1.8;margin-top:26px}
@media(max-width:760px){.contact-layout{grid-template-columns:1fr;gap:32px}.journal-form{padding:20px}}
</style>
