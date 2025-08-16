# Index.html-
Demo

<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Onaixy — Live Launch</title>
  <meta name="description" content="Onaixy — Simple GitHub Pages + Firebase launch in one HTML." />
  <meta name="theme-color" content="#5b7cfa" />

  <style>
    :root{
      --bg:#0f172a; --panel:#111827; --card:#0b1222; --text:#e5e7eb; --muted:#9ca3af; --brand:#5b7cfa; --brand2:#22d3ee; --ok:#22c55e; --warn:#f59e0b;
    }
    *{box-sizing:border-box} html,body{margin:0;height:100%}
    body{font-family:Inter,system-ui,Segoe UI,Roboto,Arial,sans-serif;background: radial-gradient(1200px 600px at 10% -10%, rgba(91,124,250,.25), transparent 40%), radial-gradient(900px 400px at 110% 0%, rgba(34,211,238,.25), transparent 30%), var(--bg); color:var(--text)}
    a{color:var(--brand); text-decoration:none}
    header{position:sticky; top:0; backdrop-filter: blur(10px); background:rgba(15,23,42,.6); border-bottom:1px solid rgba(255,255,255,.06); z-index:10}
    .nav{max-width:1100px; margin:auto; display:flex; align-items:center; justify-content:space-between; padding:14px 16px}
    .brand{display:flex; align-items:center; gap:10px; font-weight:800; letter-spacing:.5px}
    .brand .logo{width:34px; height:34px; border-radius:10px; background:linear-gradient(135deg,var(--brand),var(--brand2)); display:grid; place-items:center; color:#fff; font-weight:900}
    .links{display:flex; gap:14px; align-items:center}
    .links a{padding:8px 12px; border-radius:10px; color:var(--text)}
    .links a.active,.links a:hover{background:rgba(255,255,255,.06)}
    .cta{background:linear-gradient(135deg,var(--brand),var(--brand2)); color:#fff !important; padding:10px 14px; border-radius:11px; font-weight:700}
    .hero{max-width:1100px; margin:40px auto; padding:0 16px; display:grid; gap:14px; text-align:center}
    .title{font-size:clamp(28px,5vw,44px); font-weight:900; line-height:1.1}
    .subtitle{color:var(--muted)}
    .grid{max-width:1100px; margin:26px auto; padding:0 16px; display:grid; grid-template-columns:repeat(12,1fr); gap:16px}
    .card{grid-column: span 6; background:linear-gradient(180deg, rgba(255,255,255,.04), rgba(255,255,255,.02)); border:1px solid rgba(255,255,255,.06); padding:18px; border-radius:16px}
    .card h3{margin:0 0 6px 0}
    @media (max-width:820px){ .card{grid-column: span 12} .links{display:none} .menu-btn{display:inline-flex} }
    .menu-btn{display:none; gap:8px; align-items:center; background:transparent; color:var(--text); border:1px solid rgba(255,255,255,.12); padding:8px 10px; border-radius:10px}
    .mobile-menu{display:none; padding:10px 16px; background:rgba(15,23,42,.9); border-bottom:1px solid rgba(255,255,255,.06)}
    .mobile-menu a{display:block; padding:10px 12px; margin:6px 0; border-radius:10px; background:rgba(255,255,255,.04); color:var(--text)}
    .section{max-width:1100px; margin:40px auto; padding:0 16px}
    .kpis{display:grid; grid-template-columns:repeat(4,1fr); gap:12px}
    .kpis .k{background:rgba(255,255,255,.04); border:1px solid rgba(255,255,255,.06); padding:14px; border-radius:16px; text-align:center}
    @media (max-width:820px){ .kpis{grid-template-columns:repeat(2,1fr)} }
    details{background:rgba(255,255,255,.04); border:1px solid rgba(255,255,255,.06); padding:14px 14px; border-radius:14px}
    details+details{margin-top:14px}
    summary{cursor:pointer; font-weight:700}
    pre{background:#0b1222; color:#e5e7eb; padding:14px; border-radius:12px; overflow:auto; border:1px solid rgba(255,255,255,.08)}
    .row{display:flex; gap:10px; align-items:center; flex-wrap:wrap}
    .btn{border:1px solid rgba(255,255,255,.18); background:rgba(255,255,255,.06); color:var(--text); padding:8px 10px; border-radius:10px; cursor:pointer}
    .ok{color:var(--ok)} .warn{color:var(--warn)}
    footer{border-top:1px solid rgba(255,255,255,.08); margin-top:40px; padding:18px; text-align:center; color:var(--muted)}
    .badge{display:inline-block; padding:6px 10px; border-radius:999px; background:rgba(91,124,250,.12); color:#cdd6ff; border:1px solid rgba(91,124,250,.35); font-size:.85rem}
    .pill{display:inline-block; padding:6px 10px; border-radius:999px; background:rgba(34,211,238,.12); color:#baf6ff; border:1px solid rgba(34,211,238,.35); font-size:.85rem}
    .mono{font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace}
  </style>
</head>
<body>
  <!-- NAV -->
  <header>
    <div class="nav">
      <div class="brand">
        <div class="logo">Ω</div>
        <span>Onaixy</span>
      </div>
      <nav class="links">
        <a href="#home" class="active">Home</a>
        <a href="#features">Features</a>
        <a href="#deploy">Deploy</a>
        <a href="#contact">Contact</a>
        <a class="cta" href="#go-live">Go Live</a>
      </nav>
      <button class="menu-btn" id="menuBtn">☰ Menu</button>
    </div>
    <div class="mobile-menu" id="mobileMenu">
      <a href="#home">Home</a>
      <a href="#features">Features</a>
      <a href="#deploy">Deploy</a>
      <a href="#contact">Contact</a>
      <a class="cta" href="#go-live">Go Live</a>
    </div>
  </header>

  <!-- HERO -->
  <section id="home" class="hero">
    <span class="badge">Budget Friendly Launch · ₹12,000 Ready</span>
    <h1 class="title">Simple Launch for <span style="background:linear-gradient(90deg,var(--brand),var(--brand2)); -webkit-background-clip:text; color:transparent;">Onaixy</span></h1>
    <p class="subtitle">Static GitHub Pages + Optional Firebase backend. सब कुछ एक ही HTML में।</p>
    <div class="row" style="justify-content:center; gap:8px; margin-top:6px">
      <button class="btn" onclick="scrollToId('deploy')">Deploy Steps ↓</button>
      <button class="btn" onclick="copyQuickStart()">Copy Quick Start</button>
    </div>
  </section>

  <!-- KPIs / Highlights -->
  <div class="section">
    <div class="kpis">
      <div class="k"><div class="pill">Free Hosting</div><h3>GitHub Pages</h3><div class="subtitle">Zero server, fast CDN</div></div>
      <div class="k"><div class="pill">Optional</div><h3>Firebase</h3><div class="subtitle">Auth + Firestore + Hosting</div></div>
      <div class="k"><div class="pill">1-file</div><h3>All-in-HTML</h3><div class="subtitle">Single deploy</div></div>
      <div class="k"><div class="pill">Go Live</div><h3>~5 min</h3><div class="subtitle">From repo to URL</div></div>
    </div>
  </div>

  <!-- FEATURES -->
  <section id="features" class="grid">
    <div class="card">
      <h3>⚡ AI-Ready (Frontend)</h3>
      <p>Landing + sections + copy buttons. Ailley/AI endpoints later जोड़ें — serverless functions recommended.</p>
    </div>
    <div class="card">
      <h3>🔒 Security Basics</h3>
      <p>Static Pages → low attack surface. Firebase Auth जोड़ने पर protected routes बना सकते हैं (SPA setup में).</p>
    </div>
    <div class="card">
      <h3>🌍 Multilingual</h3>
      <p>Hindi + English UI text ready. i18n JSON add करके expand करें.</p>
    </div>
    <div class="card">
      <h3>🚀 Upgrade Path</h3>
      <p>Later: Vite + React, Netlify/Vercel, custom domain <span class="mono">onaixy.com</span>.</p>
    </div>
  </section>

  <!-- DEPLOY GUIDE -->
  <section id="deploy" class="section">
    <h2>🚀 Deploy — Saare Steps (GitHub Pages + Firebase)</h2>

    <details open>
      <summary>① GitHub Pages — Static Live (Recommended for start)</summary>
      <p class="subtitle">बस repo बनाओ, index.html upload करो, Pages on करो—live URL मिल जाएगा.</p>
      <pre><code class="mono"># 1) GitHub par new public repo banao (e.g., onaixy-live)
# 2) index.html ko root me upload/commit karo
# 3) Settings → Pages → "Deploy from a branch"
#    Branch: main, Folder: / (root) → Save
# 4) Live URL: https://USERNAME.github.io/REPO_NAME/</code></pre>
    </details>

    <details>
      <summary>② Firebase Hosting — Optional (custom domain/SSR future)</summary>
      <p class="subtitle">Firebase CLI से deploy. बाद में Auth/DB जोड़ना आसान.</p>
      <pre><code class="mono">npm install -g firebase-tools
firebase login
firebase init hosting
# ? public directory:  .   (current folder)
# ? single-page app:   n

firebase deploy
# URL: https://PROJECT_ID.web.app</code></pre>
    </details>

    <details>
      <summary>③ GitHub → Firebase Auto-Deploy (CI/CD)</summary>
      <p class="subtitle">हर push पर auto live. नीचे yml को repo में रखें: <span class="mono">.github/workflows/firebase-deploy.yml</span></p>
      <pre><code class="mono">name: Deploy to Firebase Hosting
on:
  push:
    branches: [main]
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with: { node-version: 20 }
      - run: npm install -g firebase-tools
      - run: firebase deploy --token ${{ secrets.FIREBASE_TOKEN }}</code></pre>
      <p class="subtitle">Token banane ke liye: <span class="mono">firebase login:ci</span> → token ko repo secrets me <b>FIREBASE_TOKEN</b> naam se add karo.</p>
    </details>

    <details>
      <summary>④ (Optional) Firebase Config placeholders</summary>
      <p class="subtitle">Aap आगे Auth/DB use करोगे तो ye config JS में लगाओ—abhi ये सिर्फ placeholder है.</p>
      <pre><code class="mono">&lt;script type="module"&gt;
// import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.5/firebase-app.js";
// const firebaseConfig = {
//   apiKey: "YOUR_API_KEY",
//   authDomain: "YOUR_PROJECT.firebaseapp.com",
//   projectId: "YOUR_PROJECT_ID",
//   storageBucket: "YOUR_PROJECT.appspot.com",
//   messagingSenderId: "YOUR_SENDER_ID",
//   appId: "YOUR_APP_ID"
// };
// const app = initializeApp(firebaseConfig);
&lt;/script&gt;</code></pre>
    </details>
  </section>

  <!-- CONTACT -->
  <section id="contact" class="section">
    <h2>📬 Contact / Support</h2>
    <p class="subtitle">Launch me help chahiye? Aap apna GitHub URL bhejiye, main quick audit karke steps verify kara dunga.</p>
    <div class="row" style="margin-top:8px">
      <button class="btn" onclick="copyEmail()">Copy Email</button>
      <button class="btn" onclick="copyIssue()">Copy Issue Template</button>
    </div>
  </section>

  <section id="go-live" class="section">
    <details open>
      <summary>⚡ Quick Start — Copy aur run karo</summary>
      <pre id="qs"><code class="mono"># Local folder me index.html save karo → GitHub par push:
git init
git add index.html
git commit -m "Onaixy first live"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO_NAME.git
git push -u origin main
# Repo Settings → Pages → main / (root) → Save → Done!</code></pre>
      <div class="row"><button class="btn" onclick="copyNode('qs')">Copy</button></div>
    </details>
  </section>

  <footer>© <span id="y"></span> Onaixy · Simple Launch · All-in-HTML</footer>

  <script>
    // mobile menu
    const mBtn = document.getElementById('menuBtn');
    const mMenu = document.getElementById('mobileMenu');
    if(mBtn){
      mBtn.addEventListener('click', ()=> {
        mMenu.style.display = (mMenu.style.display === 'block') ? 'none' : 'block';
      });
    }
    // year
    document.getElementById('y').textContent = new Date().getFullYear();

    // helpers
    function copy(text){
      navigator.clipboard.writeText(text).then(()=>alert('Copied!'));
    }
    function copyNode(id){
      const t = document.getElementById(id)?.innerText || '';
      copy(t);
    }
    function copyQuickStart(){
      copy(document.getElementById('qs').innerText);
    }
    function copyEmail(){
      copy('support@onaixy.com');
    }
    function copyIssue(){
      copy(`Title: Live Deploy Help
Repo: https://github.com/USERNAME/REPO_NAME
What I did: Pages enabled (main / root)
What I see: (paste screenshot)
What I expect: Live homepage visible`);
    }
    function scrollToId(id){
      const el = document.getElementById(id);
      if(el) el.scrollIntoView({behavior:'smooth', block:'start'});
    }
  </script>
</body>
</html>
