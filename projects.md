---
permalink: /projects/
layout: default
title: Books
---

<article class="content-page reveal library-page">
  <div class="eyebrow">A little shelf of stories</div>
  <h1>My little library.</h1>
  <p class="library-intro">A few stories, ideas and little worlds waiting on my shelves. This library is still growing, one book at a time.</p>
  <div class="library-decor" aria-hidden="true"><span>✳</span><span>✿</span><span>“</span></div>
  <section class="library-room" aria-label="Book collection">
    <div class="library-shelf">
      <div class="shelf-row">
        <div class="library-book book-coral"><span class="book-number">01</span><strong>Book title</strong><small>author soon</small></div>
        <div class="library-book book-blue"><span class="book-number">02</span><strong>Another story</strong><small>author soon</small></div>
        <div class="library-book book-sage"><span class="book-number">03</span><strong>A new chapter</strong><small>author soon</small></div>
        <div class="library-book book-lilac"><span class="book-number">04</span><strong>Little worlds</strong><small>author soon</small></div>
        <div class="library-book book-gold"><span class="book-number">05</span><strong>On my list</strong><small>author soon</small></div>
        <div class="library-book book-teal"><span class="book-number">06</span><strong>More to read</strong><small>author soon</small></div>
      </div>
      <div class="shelf-plank"><span></span></div>
      <div class="shelf-row second-row">
        <div class="library-book book-lilac"><span class="book-number">07</span><strong>Next adventure</strong><small>author soon</small></div>
        <div class="library-book book-gold"><span class="book-number">08</span><strong>Quiet pages</strong><small>author soon</small></div>
        <div class="library-book book-teal"><span class="book-number">09</span><strong>Somewhere new</strong><small>author soon</small></div>
        <div class="library-book book-coral"><span class="book-number">10</span><strong>To be read</strong><small>author soon</small></div>
        <div class="library-book book-blue"><span class="book-number">11</span><strong>One more tale</strong><small>author soon</small></div>
        <div class="library-book book-sage"><span class="book-number">12</span><strong>Coming soon</strong><small>author soon</small></div>
      </div>
      <div class="shelf-plank"><span></span></div>
    </div>
  </section>
  <p class="library-footnote">The titles are placeholders for now. The real collection will find its place here soon. <span>♡</span></p>
</article>

<style>
  .library-page{max-width:980px;position:relative;overflow:hidden}
  .library-intro{max-width:690px}
  .library-decor{position:absolute;right:8%;top:7%;display:flex;gap:20px;color:#d49b83;font:2rem var(--caveat);transform:rotate(8deg)}
  .library-decor span:nth-child(2){color:#9b88b7;transform:translateY(20px) rotate(-15deg)}
  .library-decor span:nth-child(3){font-size:4rem;color:#d9b96e}
  .library-room{margin:36px 0 22px;padding:28px 22px 10px;border:2px solid #eadcc9;border-radius:18px;background:linear-gradient(145deg,#f5e8d8,#fff8ed 48%,#f1e3d3);box-shadow:inset 0 0 35px rgba(137,103,77,.08),7px 9px 0 rgba(201,183,232,.22);perspective:1200px}
  .library-shelf{position:relative;padding:8px 13px 0;background:linear-gradient(90deg,rgba(132,91,69,.08),transparent 12%,transparent 88%,rgba(132,91,69,.08))}
  .shelf-row{min-height:190px;display:flex;align-items:flex-end;justify-content:center;gap:clamp(5px,1.5vw,16px);padding:12px 4px 0;transform-style:preserve-3d}
  .library-book{--book:#c87869;position:relative;isolation:isolate;flex:1 1 0;max-width:112px;min-width:0;height:clamp(125px,17vw,174px);padding:13px 8px 11px;display:flex;flex-direction:column;align-items:center;justify-content:space-between;text-align:center;color:#fff9ed;border-radius:5px 9px 2px 2px;background:linear-gradient(90deg,rgba(50,35,35,.28),rgba(255,255,255,.14) 12%,transparent 28%,rgba(40,30,30,.12) 100%),var(--book);box-shadow:inset 4px 0 5px rgba(255,255,255,.18),inset -4px 0 5px rgba(55,35,30,.13),5px 7px 10px rgba(64,59,80,.17);transform:rotateY(-5deg) translateZ(0);transform-origin:bottom center;transition:transform .45s cubic-bezier(.2,.8,.2,1),box-shadow .45s;cursor:default}
  .library-book:before{content:"";position:absolute;inset:7px 6px;border:1px solid rgba(255,249,237,.38);border-radius:3px;pointer-events:none}
  .library-book:after{content:"";position:absolute;left:8px;top:0;bottom:0;width:1px;background:rgba(255,255,255,.25);box-shadow:2px 0 3px rgba(40,20,20,.1)}
  .library-book strong{font:700 clamp(1.05rem,2vw,1.45rem)/.92 var(--caveat);max-width:100%;overflow-wrap:anywhere;position:relative;z-index:1}
  .library-book small{font:1rem/1 var(--hand);opacity:.88;position:relative;z-index:1}
  .book-number{font:600 1rem var(--caveat);opacity:.85;align-self:flex-start;position:relative;z-index:1}
  .library-book:hover{transform:translateY(-13px) rotateY(-14deg) rotateX(4deg) scale(1.035);box-shadow:inset 4px 0 5px rgba(255,255,255,.18),inset -4px 0 5px rgba(55,35,30,.13),12px 17px 17px rgba(64,59,80,.2);z-index:3}
  .book-coral{--book:#c87569;height:clamp(133px,18vw,181px)}.book-blue{--book:#687f9f;height:clamp(145px,19vw,190px)}.book-sage{--book:#78947a;height:clamp(128px,16vw,166px)}.book-lilac{--book:#9b80ad;height:clamp(151px,20vw,198px)}.book-gold{--book:#b58d4d;height:clamp(137px,18vw,178px)}.book-teal{--book:#56858a;height:clamp(147px,19vw,190px)}
  .shelf-plank{height:17px;position:relative;margin:0 -7px;background:linear-gradient(180deg,#d4a982 0%,#bd8d68 35%,#9f7054 100%);border-radius:3px 3px 7px 7px;box-shadow:0 7px 9px rgba(92,63,47,.2),inset 0 2px 2px rgba(255,255,255,.42),inset 0 -3px 3px rgba(84,51,37,.18);z-index:4}
  .shelf-plank span{position:absolute;left:2%;right:2%;top:4px;height:1px;background:rgba(255,244,222,.4)}
  .second-row{padding-top:15px}
  .library-footnote{text-align:center;font:1.45rem var(--caveat);color:#887a8f;margin:28px 0 0}
  .library-footnote span{color:#cf8176;font-size:1.7rem}
  @media(max-width:680px){.library-decor{top:4%;right:7%;gap:10px;font-size:1.5rem}.library-decor span:nth-child(3){font-size:2.8rem}.library-room{margin:26px -5px 18px;padding:18px 8px 8px}.library-shelf{padding:5px 3px 0}.shelf-row{min-height:145px;gap:4px;padding:8px 1px 0}.library-book{height:clamp(105px,29vw,145px);padding:9px 3px 8px;border-radius:4px 6px 2px 2px}.library-book strong{font-size:clamp(.88rem,3.3vw,1.15rem)}.library-book small{font-size:.78rem}.book-number{font-size:.82rem}.book-coral{height:clamp(110px,30vw,150px)}.book-blue{height:clamp(120px,33vw,160px)}.book-sage{height:clamp(104px,28vw,140px)}.book-lilac{height:clamp(124px,34vw,165px)}.book-gold{height:clamp(113px,31vw,151px)}.book-teal{height:clamp(120px,33vw,160px)}.shelf-plank{height:13px;margin:0 -3px}.second-row{padding-top:12px}}
  @media(max-width:390px){.library-room{padding-left:5px;padding-right:5px}.shelf-row{gap:3px}.library-book{padding-left:2px;padding-right:2px}.library-book strong{font-size:.83rem}.library-book small{font-size:.7rem}}
  @media(prefers-reduced-motion:reduce){.library-book{transition:none}}
</style>
