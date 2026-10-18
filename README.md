<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#fff0f5">
<title>For Ashley ♡</title>
<style>
  :root { --pink:#ff6f9f; --deep:#a83261; --cream:#fff8f7; --ink:#563344; }
  * { box-sizing:border-box; }
  html { scroll-behavior:smooth; }
  body {
    margin:0; min-height:100vh; color:var(--ink);
    font-family: ui-rounded, "Trebuchet MS", system-ui, sans-serif;
    background: radial-gradient(circle at 15% 15%, #ffe0ec 0, transparent 30%),
                radial-gradient(circle at 85% 30%, #ffe9d9 0, transparent 28%),
                linear-gradient(145deg,#fff8fb,#fff0f5 55%,#fff9f0);
    overflow-x:hidden;
  }
  .floaties { position:fixed; inset:0; pointer-events:none; overflow:hidden; z-index:0; }
  .floaty { position:absolute; bottom:-50px; opacity:.42; animation: rise linear infinite; }
  @keyframes rise { to { transform:translateY(-115vh) rotate(25deg); opacity:0; } }
  main { position:relative; z-index:1; }
  .hero { min-height:92vh; display:grid; place-items:center; padding:48px 18px 60px; text-align:center; }
  .hero-inner { max-width:760px; }
  .eyebrow { display:inline-block; padding:9px 15px; border:1px solid #ffc1d5; border-radius:999px; background:#ffffffb8; color:var(--deep); font-size:.86rem; letter-spacing:.06em; }
  h1 { margin:22px 0 12px; font-size:clamp(3.2rem,12vw,7rem); line-height:.98; letter-spacing:-.065em; color:var(--deep); }
  h1 span { color:var(--pink); }
  .lead { max-width:560px; margin:0 auto; font-size:clamp(1.05rem,3vw,1.3rem); line-height:1.8; }
  .actions { display:flex; gap:12px; justify-content:center; flex-wrap:wrap; margin-top:28px; }
  button, .button { cursor:pointer; border:0; border-radius:999px; padding:14px 22px; font:inherit; font-weight:700; transition:transform .2s, box-shadow .2s; }
  button:hover, .button:hover { transform:translateY(-3px); box-shadow:0 10px 24px #d65b8533; }
  .primary { background:linear-gradient(135deg,#ff6f9f,#e94e87); color:white; box-shadow:0 7px 18px #e94e8730; }
  .secondary { color:var(--deep); background:#fff; border:1px solid #ffd1df; }
  .hint { margin-top:17px; font-size:.88rem; opacity:.72; }
  section { padding:55px 18px; }
  .section-inner { max-width:960px; margin:auto; }
  .section-title { text-align:center; color:var(--deep); font-size:clamp(2rem,6vw,3.2rem); margin:0 0 12px; letter-spacing:-.04em; }
  .section-sub { text-align:center; max-width:600px; margin:0 auto 30px; line-height:1.7; opacity:.8; }
  .cards { display:grid; grid-template-columns:repeat(3,minmax(0,1fr)); gap:16px; }
  .card { padding:25px 22px; background:#ffffffc9; border:1px solid #ffe0e9; border-radius:24px; box-shadow:0 12px 35px #8b36500b; }
  .card .emoji { font-size:2rem; }
  .card h3 { color:var(--deep); margin:12px 0 8px; }
  .card p { line-height:1.7; margin:0; }
  .letter { max-width:700px; margin:auto; background:#fffdfd; border:1px solid #ffdce7; border-radius:28px; padding:clamp(25px,6vw,48px); box-shadow:0 20px 55px #8b365010; position:relative; }
  .letter:before { content:"♡"; position:absolute; top:15px; right:22px; font-size:2rem; color:#ffb0ca; }
  .letter p { font-size:1.06rem; line-height:1.95; }
  .signature { color:var(--deep); font-size:1.35rem; font-weight:800; }
  .surprise-wrap { text-align:center; }
  #surprise { display:none; max-width:620px; margin:25px auto 0; padding:25px; background:#fff; border:1px dashed #ff9fbe; border-radius:24px; line-height:1.9; animation:pop .45s ease-out; }
  @keyframes pop { from { opacity:0; transform:scale(.94); } to { opacity:1; transform:scale(1); } }
  footer { padding:32px 18px 45px; text-align:center; opacity:.72; font-size:.9rem; }
  .heart { display:inline-block; color:#ed5a8c; animation:beat 1s infinite; }
  @keyframes beat { 50% { transform:scale(1.22); } }
  .sprinkle { position:fixed; top:-30px; z-index:5; pointer-events:none; animation:fall 2.8s linear forwards; }
  @keyframes fall { to { transform:translateY(110vh) rotate(650deg); opacity:.15; } }
  @media(max-width:700px) { .cards { grid-template-columns:1fr; } .card { padding:22px; } .hero { min-height:88vh; } }
  @media(prefers-reduced-motion:reduce) { *,*::before,*::after { animation-duration:.01ms!important; animation-iteration-count:1!important; scroll-behavior:auto!important; } }
</style>
</head>
<body>
<div class="floaties" id="floaties" aria-hidden="true"></div>
<main>
  <header class="hero">
    <div class="hero-inner">
      <div class="eyebrow">A little corner of the internet, just for you ♡</div>
      <h1>For <span>Ashley</span></h1>
      <p class="lead">If I could turn all the affection I feel into something you could see, it might look a little like this.</p>
      <div class="actions">
        <button class="primary" onclick="document.getElementById('letter-section').scrollIntoView({behavior:'smooth'})">Open your letter 💌</button>
        <button class="secondary" onclick="showSurprise()">A tiny surprise ✨</button>
      </div>
      <p class="hint">Made with care, and a whole lot of heart.</p>
    </div>
  </header>

  <section aria-labelledby="little-things">
    <div class="section-inner">
      <h2 class="section-title" id="little-things">A few things I hope you feel</h2>
      <p class="section-sub">Not every feeling fits neatly into words, but these are some of the things I want you to know.</p>
      <div class="cards">
        <article class="card"><div class="emoji">🌷</div><h3>You matter</h3><p>Your presence can make an ordinary day feel a little more special. I hope you never forget how important you are.</p></article>
        <article class="card"><div class="emoji">☀️</div><h3>You bring warmth</h3><p>There is something lovely about you that makes the world feel softer and brighter. You deserve that same kindness back.</p></article>
        <article class="card"><div class="emoji">🫶</div><h3>You are appreciated</h3><p>For the little things, the big things, and simply being yourself—thank you for being someone worth caring about.</p></article>
      </div>
    </div>
  </section>

  <section id="letter-section">
    <div class="section-inner">
      <h2 class="section-title">A letter for you</h2>
      <p class="section-sub">A few words from my heart to yours.</p>
      <div class="letter">
        <p>Dear Ashley,</p>
        <p>I made this little page because sometimes a simple message doesn't feel like enough to express how much affection one person can hold for another.</p>
        <p>I want you to know that you deserve to feel cared for, valued, and appreciated—not just on the happiest days, but on the quiet and difficult ones too. I hope I can bring a smile to your face, give you reasons to laugh, and remind you that you are someone truly special.</p>
        <p>No fancy words could ever capture every feeling perfectly. So here's the honest part: I'm glad you're you, Ashley. And I'm happy I get to tell you that.</p>
        <p>Whenever you need a little reminder, come back to this page and remember that someone made it just to put a smile on your face. ♡</p>
        <p class="signature">With lots of affection, <span class="heart">♥</span></p>
      </div>
    </div>
  </section>

  <section>
    <div class="section-inner surprise-wrap">
      <h2 class="section-title">One last little thing…</h2>
      <p class="section-sub">Because you deserve a surprise just for being you.</p>
      <button class="primary" onclick="showSurprise()">Tap for a little happiness 💗</button>
      <div id="surprise" role="status" aria-live="polite">
        <div style="font-size:2.3rem">💖🌸✨</div>
        <strong>Ashley, here's your reminder:</strong><br>
        You are appreciated more than you know. I hope something wonderful happens to you today, that you find a reason to smile, and that you always remember how deserving you are of love, gentleness, and happiness. Sending you the biggest virtual hug! 🫂
      </div>
    </div>
  </section>
  <footer>Made especially for Ashley <span class="heart">♥</span><br><span style="font-size:.8rem">A small page for a very special person.</span></footer>
</main>
<script>
  const floaties = document.getElementById('floaties');
  const symbols = ['♡','♥','✦','✿'];
  for (let i=0; i<18; i++) {
    const el = document.createElement('span');
    el.className = 'floaty';
    el.textContent = symbols[Math.floor(Math.random()*symbols.length)];
    el.style.left = Math.random()*100 + '%';
    el.style.fontSize = (14+Math.random()*22)+'px';
    el.style.animationDuration = (9+Math.random()*12)+'s';
    el.style.animationDelay = (-Math.random()*18)+'s';
    floaties.appendChild(el);
  }
  function showSurprise() {
    const panel = document.getElementById('surprise');
    panel.style.display = 'block';
    panel.scrollIntoView({behavior:'smooth', block:'center'});
    for (let i=0; i<32; i++) {
      const el = document.createElement('span');
      el.className = 'sprinkle';
      el.textContent = symbols[Math.floor(Math.random()*symbols.length)];
      el.style.left = Math.random()*100 + 'vw';
      el.style.fontSize = (12+Math.random()*20)+'px';
      el.style.color = ['#ff6f9f','#c15a90','#f5a65b','#a83261'][Math.floor(Math.random()*4)];
      el.style.animationDuration = (1.8+Math.random()*1.8)+'s';
      document.body.appendChild(el);
      setTimeout(()=>el.remove(), 4000);
    }
  }
</script>
</body>
</html>
