<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Rose — Home</title>
  <meta name="description" content="Rose — project front page" />

  <!-- Simple, self-contained styles -->
  <style>
    :root{
      --accent:#e84a5f;
      --dark:#0f1724;
      --muted:#9aa4b2;
      --card:#ffffff;
      --bg: linear-gradient(135deg,#0f1724 0%, #1b2a41 100%);
      --glass: rgba(255,255,255,0.06);
      --radius:12px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    html,body{height:100%}
    body{
      margin:0;
      background:var(--bg);
      color:#eef2f7;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.45;
      display:flex;
      flex-direction:column;
      min-height:100vh;
    }

    .container{
      width:min(1100px,92%);
      margin:0 auto;
      padding:48px 0;
      flex:1;
    }

    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
      margin-bottom:28px;
    }
    .brand{
      display:flex;
      gap:12px;
      align-items:center;
      text-decoration:none;
      color:inherit;
    }
    .logo{
      width:56px;
      height:56px;
      border-radius:12px;
      background:linear-gradient(135deg,#fff3 0%, #fff1 60%), #ffffff10;
      display:grid;
      place-items:center;
      font-weight:700;
      color:var(--accent);
      border:1px solid rgba(255,255,255,0.06);
      box-shadow: 0 6px 20px rgba(0,0,0,0.4), inset 0 -2px 6px rgba(255,255,255,0.02);
      font-size:20px;
    }
    nav a{
      color:var(--muted);
      text-decoration:none;
      margin-left:18px;
      font-weight:600;
    }
    .hero{
      display:grid;
      grid-template-columns:1fr 380px;
      gap:32px;
      align-items:center;
      margin-top:18px;
    }
    .hero-card{
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:var(--radius);
      padding:32px;
      box-shadow: 0 8px 30px rgba(2,6,23,0.6);
      border:1px solid rgba(255,255,255,0.04);
    }
    h1{
      margin:0 0 12px 0;
      font-size:34px;
      letter-spacing:-0.02em;
    }
    p.lead{
      margin:0 0 20px 0;
      color:var(--muted);
      font-size:16px;
    }
    .actions{
      display:flex;
      gap:12px;
    }
    .btn{
      display:inline-flex;
      align-items:center;
      gap:10px;
      padding:10px 16px;
      border-radius:10px;
      background:var(--card);
      color:var(--dark);
      font-weight:700;
      text-decoration:none;
      box-shadow: 0 6px 18px rgba(2,6,23,0.45);
      border:0;
    }
    .btn.secondary{
      background:transparent;
      color:var(--card);
      border:1px solid rgba(255,255,255,0.06);
      font-weight:600;
    }

    .right-panel{
      display:flex;
      flex-direction:column;
      gap:14px;
    }

    .stat{
      background:var(--glass);
      padding:16px;
      border-radius:12px;
      border:1px solid rgba(255,255,255,0.04);
      text-align:center;
    }
    .stat strong{display:block;font-size:20px;color:#fff}
    .features{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
      gap:16px;
      margin-top:28px;
    }
    .card{
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      padding:18px;
      border-radius:12px;
      border:1px solid rgba(255,255,255,0.03);
    }
    footer{
      margin-top:40px;
      padding:20px 0;
      color:var(--muted);
      text-align:center;
      font-size:14px;
    }

    /* Responsive */
    @media (max-width:900px){
      .hero{grid-template-columns:1fr; padding-bottom:14px}
      .right-panel{flex-direction:row; flex-wrap:wrap}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <a class="brand" href="/">
        <div class="logo">R</div>
        <div>
          <div style="font-weight:800">Rose</div>
          <div style="font-size:12px;color:var(--muted)">A short tagline or one-line description</div>
        </div>
      </a>

      <nav>
        <a href="#features">Features</a>
        <a href="#docs">Docs</a>
        <a href="#community">Community</a>
        <a class="btn secondary" href="https://github.com/vrutantkar550-png/Rose" target="_blank" rel="noopener">View on GitHub</a>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div class="hero-card">
          <h1>Rose — elegant, modern starter for your project</h1>
          <p class="lead">
            Clean UI, accessible components, and a simple developer experience — drop this front page into your repo and adapt quickly.
          </p>

          <div class="actions">
            <a class="btn" href="#get-started">Get Started</a>
            <a class="btn secondary" href="https://github.com/vrutantkar550-png/Rose" target="_blank" rel="noopener">Open repo</a>
          </div>

          <div id="get-started" style="margin-top:20px;color:var(--muted);font-size:14px">
            <strong>Install</strong>
            <div style="margin-top:8px">Copy this file to your repo as <code>index.html</code>. If you want a static site, enable GitHub Pages on this repository and set the source to the main branch.</div>
          </div>
        </div>

        <aside class="right-panel">
          <div class="stat">
            <div style="font-size:12px;color:var(--muted)">Version</div>
            <strong>0.1.0</strong>
          </div>

          <div class="stat">
            <div style="font-size:12px;color:var(--muted)">License</div>
            <strong>MIT</strong>
          </div>

          <div class="stat">
            <div style="font-size:12px;color:var(--muted)">Languages</div>
            <strong>HTML / CSS / JS</strong>
          </div>
        </aside>
      </section>

      <section id="features" style="margin-top:28px">
        <h2 style="margin-bottom:12px">Features</h2>
        <div class="features">
          <div class="card">
            <h3 style="margin-top:0">Responsive</h3>
            <p style="margin:6px 0;color:var(--muted)">Works well on phones, tablets, and desktops without extra libraries.</p>
          </div>

          <div class="card">
            <h3 style="margin-top:0">Lightweight</h3>
            <p style="margin:6px 0;color:var(--muted)">No heavy frameworks — plain HTML/CSS with a few small helpers if needed.</p>
          </div>

          <div class="card">
            <h3 style="margin-top:0">Customizable</h3>
            <p style="margin:6px 0;color:var(--muted)">Easy to adapt colors, fonts, and layout to match your brand.</p>
          </div>
        </div>
      </section>

      <section id="community" style="margin-top:32px">
        <h2 style="margin-bottom:12px">Contribute</h2>
        <p style="color:var(--muted);margin:0 0 12px 0">Contributions, issues, and suggestions are welcome. Open a PR or an issue on GitHub.</p>
        <div style="display:flex;gap:10px;flex-wrap:wrap;margin-top:8px">
          <a class="btn" href="https://github.com/vrutantkar550-png/Rose/issues" target="_blank" rel="noopener">Report an issue</a>
          <a class="btn secondary" href="https://github.com/vrutantkar550-png/Rose/pulls" target="_blank" rel="noopener">Open a PR</a>
        </div>
      </section>
    </main>

    <footer>
      Made with ❤️ — <a href="https://github.com/vrutantkar550-png/Rose" target="_blank" style="color:inherit;text-decoration:underline">vrutantkar550-png/Rose</a>
    </footer>
  </div>

  <!-- Minimal JS for example: copy-to-clipboard or future enhancements -->
  <script>
    // Placeholder: you can add small interactions here if needed.
  </script>
</body>
</html># Rose
