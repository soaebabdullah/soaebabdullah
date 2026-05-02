[![MasterHead](https://www.vackergroup.ae/wp-content/uploads/2016/04/Iot-cover-image.gif)](https://www.linkedin.com/in/soaeb-abdullah/)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Soaeb Abdullah — Software Engineer</title>
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=Fraunces:ital,opsz,wght@0,9..144,300;0,9..144,600;1,9..144,300&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet" />
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --bg: #0e0f11;
    --surface: #161719;
    --surface2: #1e2023;
    --border: rgba(255,255,255,0.07);
    --border2: rgba(255,255,255,0.12);
    --text: #e8e6e1;
    --muted: #7a7875;
    --accent: #1D9E75;
    --accent-dim: #0f6e56;
    --accent-glow: rgba(29,158,117,0.12);
    --mono: 'DM Mono', monospace;
    --serif: 'Fraunces', serif;
    --sans: 'DM Sans', sans-serif;
  }

  html { scroll-behavior: smooth; }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: var(--sans);
    font-size: 15px;
    line-height: 1.7;
    min-height: 100vh;
    overflow-x: hidden;
  }

  /* ── layout ── */
  .page {
    max-width: 780px;
    margin: 0 auto;
    padding: 0 24px 80px;
  }

  /* ── top nav bar ── */
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 28px 0 0;
    margin-bottom: 80px;
    animation: fadeUp 0.6s ease both;
  }

  .nav-logo {
    font-family: var(--mono);
    font-size: 13px;
    color: var(--accent);
    letter-spacing: 0.08em;
  }

  .nav-links {
    display: flex;
    gap: 28px;
    list-style: none;
  }

  .nav-links a {
    font-family: var(--mono);
    font-size: 12px;
    color: var(--muted);
    text-decoration: none;
    letter-spacing: 0.06em;
    transition: color 0.2s;
  }

  .nav-links a:hover { color: var(--text); }

  /* ── hero ── */
  .hero {
    display: grid;
    grid-template-columns: 1fr auto;
    gap: 40px;
    align-items: end;
    margin-bottom: 72px;
  }

  .hero-eyebrow {
    font-family: var(--mono);
    font-size: 12px;
    color: var(--accent);
    letter-spacing: 0.1em;
    margin-bottom: 16px;
    display: flex;
    align-items: center;
    gap: 8px;
    animation: fadeUp 0.6s 0.1s ease both;
  }

  .hero-eyebrow::before {
    content: '';
    display: inline-block;
    width: 24px;
    height: 1px;
    background: var(--accent);
  }

  .hero-name {
    font-family: var(--serif);
    font-size: clamp(44px, 8vw, 72px);
    font-weight: 600;
    line-height: 1.0;
    letter-spacing: -0.02em;
    color: var(--text);
    animation: fadeUp 0.6s 0.15s ease both;
  }

  .hero-name em {
    font-style: italic;
    font-weight: 300;
    color: var(--accent);
  }

  .hero-sub {
    font-size: 15px;
    color: var(--muted);
    margin-top: 18px;
    max-width: 420px;
    line-height: 1.8;
    animation: fadeUp 0.6s 0.2s ease both;
  }

  .hero-status {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    margin-top: 28px;
    background: var(--accent-glow);
    border: 1px solid rgba(29,158,117,0.25);
    border-radius: 100px;
    padding: 6px 14px;
    font-family: var(--mono);
    font-size: 12px;
    color: var(--accent);
    animation: fadeUp 0.6s 0.25s ease both;
  }

  .pulse {
    width: 7px;
    height: 7px;
    border-radius: 50%;
    background: var(--accent);
    animation: pulse 2s infinite;
  }

  @keyframes pulse {
    0%, 100% { opacity: 1; transform: scale(1); }
    50% { opacity: 0.4; transform: scale(0.85); }
  }

  .avatar {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    border: 1px solid var(--border2);
    background: var(--surface2);
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: var(--serif);
    font-size: 30px;
    font-weight: 600;
    color: var(--accent);
    animation: fadeUp 0.6s 0.1s ease both;
    flex-shrink: 0;
  }

  /* ── divider ── */
  hr {
    border: none;
    border-top: 1px solid var(--border);
    margin: 48px 0;
  }

  /* ── section label ── */
  .section-tag {
    font-family: var(--mono);
    font-size: 11px;
    letter-spacing: 0.12em;
    color: var(--muted);
    text-transform: uppercase;
    margin-bottom: 24px;
  }

  /* ── code block ── */
  .code-block {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 24px 28px;
    font-family: var(--mono);
    font-size: 13px;
    line-height: 2;
    margin-bottom: 48px;
    animation: fadeUp 0.6s 0.3s ease both;
    position: relative;
    overflow: hidden;
  }

  .code-block::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 1px;
    background: linear-gradient(90deg, var(--accent), transparent);
  }

  .code-dots {
    display: flex;
    gap: 6px;
    margin-bottom: 16px;
  }

  .code-dots span {
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: var(--border2);
  }

  .code-dots span:first-child { background: #ff5f56; }
  .code-dots span:nth-child(2) { background: #ffbd2e; }
  .code-dots span:nth-child(3) { background: #27c93f; }

  .kw { color: #AFA9EC; }
  .fn { color: #5DCAA5; }
  .str { color: #FAC775; }
  .cm { color: var(--muted); font-style: italic; }
  .op { color: var(--muted); }

  /* ── stack grid ── */
  .stack-section {
    margin-bottom: 48px;
    animation: fadeUp 0.6s 0.35s ease both;
  }

  .stack-group {
    margin-bottom: 20px;
  }

  .stack-group-label {
    font-family: var(--mono);
    font-size: 11px;
    color: var(--muted);
    letter-spacing: 0.08em;
    margin-bottom: 10px;
  }

  .chips {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  .chip {
    font-family: var(--mono);
    font-size: 12px;
    padding: 5px 12px;
    border-radius: 6px;
    border: 1px solid var(--border);
    background: var(--surface);
    color: var(--text);
    transition: border-color 0.2s, color 0.2s;
    cursor: default;
  }

  .chip:hover { border-color: var(--border2); color: #fff; }

  .chip.primary {
    border-color: rgba(29,158,117,0.3);
    color: #5DCAA5;
    background: var(--accent-glow);
  }

  .chip.devops {
    border-color: rgba(239,159,39,0.25);
    color: #EF9F27;
    background: rgba(239,159,39,0.06);
  }

  .chip.lang {
    border-color: rgba(175,169,236,0.25);
    color: #AFA9EC;
    background: rgba(175,169,236,0.06);
  }

  /* ── links grid ── */
  .links-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
    margin-bottom: 48px;
    animation: fadeUp 0.6s 0.4s ease both;
  }

  .link-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 18px 20px;
    text-decoration: none;
    transition: border-color 0.2s, background 0.2s;
    display: flex;
    flex-direction: column;
    gap: 6px;
  }

  .link-card:hover {
    border-color: var(--border2);
    background: var(--surface2);
  }

  .link-card-label {
    font-family: var(--mono);
    font-size: 11px;
    color: var(--muted);
    letter-spacing: 0.08em;
  }

  .link-card-title {
    font-size: 14px;
    font-weight: 500;
    color: var(--text);
  }

  .link-card-arrow {
    font-family: var(--mono);
    font-size: 16px;
    color: var(--accent);
    margin-top: 4px;
  }

  /* ── connect row ── */
  .connect {
    display: flex;
    align-items: center;
    gap: 16px;
    animation: fadeUp 0.6s 0.45s ease both;
  }

  .connect-label {
    font-family: var(--mono);
    font-size: 12px;
    color: var(--muted);
  }

  .social-pill {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 8px 18px;
    border-radius: 100px;
    border: 1px solid rgba(29,158,117,0.35);
    background: var(--accent-glow);
    color: var(--accent);
    font-family: var(--mono);
    font-size: 13px;
    text-decoration: none;
    transition: background 0.2s, border-color 0.2s;
  }

  .social-pill:hover {
    background: rgba(29,158,117,0.2);
    border-color: var(--accent);
  }

  /* ── footer ── */
  footer {
    margin-top: 72px;
    padding-top: 28px;
    border-top: 1px solid var(--border);
    display: flex;
    justify-content: space-between;
    align-items: center;
    animation: fadeUp 0.6s 0.5s ease both;
  }

  footer p {
    font-family: var(--mono);
    font-size: 12px;
    color: var(--muted);
  }

  .flag {
    font-size: 18px;
  }

  /* ── animations ── */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(16px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  /* ── responsive ── */
  @media (max-width: 560px) {
    .hero { grid-template-columns: 1fr; }
    .avatar { display: none; }
    .links-grid { grid-template-columns: 1fr; }
    footer { flex-direction: column; gap: 8px; text-align: center; }
  }
</style>
</head>
<body>
<div class="page">

  <nav>
    <span class="nav-logo">soaeb.dev</span>
    <ul class="nav-links">
      <li><a href="https://www.linkedin.com/in/soaeb-abdullah/" target="_blank">linkedin</a></li>
      <li><a href="https://www.availabilityshare.com/" target="_blank">project</a></li>
      <li><a href="https://drive.google.com/file/d/1E0YmnXrqEETQbu_dkPykk_IkA4HQPURg/view?usp=sharing" target="_blank">resume</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div>
      <p class="hero-eyebrow">Software Engineer · Bangladesh</p>
      <h1 class="hero-name">Soaeb<br><em>Abdullah</em></h1>
      <p class="hero-sub">
        Odoo Developer &amp; DevOps Engineer. Building scalable ERP solutions and shipping production infrastructure from Dhaka.
      </p>
      <div class="hero-status">
        <span class="pulse"></span>
        Building availabilityshare.com
      </div>
    </div>
    <div class="avatar">SA</div>
  </section>

  <div class="code-block">
    <div class="code-dots"><span></span><span></span><span></span></div>
    <div><span class="cm"># about.py</span></div>
    <div><span class="kw">class</span> <span class="fn">Soaeb</span><span class="op">(</span><span class="fn">Engineer</span><span class="op">):</span></div>
    <div>&nbsp;&nbsp;role&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="op">=</span> <span class="str">"Software Engineer &amp; Tech Project Manager"</span></div>
    <div>&nbsp;&nbsp;stack&nbsp;&nbsp;&nbsp;&nbsp;<span class="op">=</span> <span class="str">"Odoo · Python · DevOps · PostgreSQL"</span></div>
    <div>&nbsp;&nbsp;learning&nbsp;<span class="op">=</span> <span class="str">"Advanced Odoo modules"</span></div>
    <div>&nbsp;&nbsp;location&nbsp;<span class="op">=</span> <span class="str">"Dhaka, Bangladesh 🇧🇩"</span></div>
  </div>

  <div class="stack-section">
    <p class="section-tag">Tech stack</p>

    <div class="stack-group">
      <p class="stack-group-label">erp &amp; backend</p>
      <div class="chips">
        <span class="chip primary">Odoo</span>
        <span class="chip primary">Python</span>
        <span class="chip primary">PostgreSQL</span>
        <span class="chip primary">MySQL</span>
      </div>
    </div>

    <div class="stack-group">
      <p class="stack-group-label">devops &amp; infra</p>
      <div class="chips">
        <span class="chip devops">Docker</span>
        <span class="chip devops">Nginx</span>
        <span class="chip devops">Linux</span>
        <span class="chip devops">AWS</span>
        <span class="chip devops">Git</span>
      </div>
    </div>

    <div class="stack-group">
      <p class="stack-group-label">languages</p>
      <div class="chips">
        <span class="chip lang">C</span>
        <span class="chip lang">C++</span>
        <span class="chip lang">C#</span>
      </div>
    </div>

    <div class="stack-group">
      <p class="stack-group-label">tools &amp; design</p>
      <div class="chips">
        <span class="chip">Bootstrap</span>
        <span class="chip">Firebase</span>
        <span class="chip">OpenCV</span>
        <span class="chip">Android</span>
        <span class="chip">Arduino</span>
        <span class="chip">Postman</span>
        <span class="chip">Figma</span>
        <span class="chip">Sketch</span>
        <span class="chip">Illustrator</span>
      </div>
    </div>
  </div>

  <div class="links-grid">
    <a class="link-card" href="https://www.availabilityshare.com/" target="_blank">
      <span class="link-card-label">current project</span>
      <span class="link-card-title">Availability Share</span>
      <span class="link-card-arrow">→</span>
    </a>
    <a class="link-card" href="https://drive.google.com/file/d/1E0YmnXrqEETQbu_dkPykk_IkA4HQPURg/view?usp=sharing" target="_blank">
      <span class="link-card-label">document</span>
      <span class="link-card-title">Resume / CV</span>
      <span class="link-card-arrow">→</span>
    </a>
    <a class="link-card" href="https://www.linkedin.com/in/soaeb-abdullah/" target="_blank">
      <span class="link-card-label">portfolio</span>
      <span class="link-card-title">Projects on LinkedIn</span>
      <span class="link-card-arrow">→</span>
    </a>
    <a class="link-card" href="https://www.linkedin.com/in/soaeb-abdullah/" target="_blank">
      <span class="link-card-label">connect</span>
      <span class="link-card-title">LinkedIn Profile</span>
      <span class="link-card-arrow">→</span>
    </a>
  </div>

  <div class="connect">
    <span class="connect-label">reach me</span>
    <a class="social-pill" href="https://www.linkedin.com/in/soaeb-abdullah/" target="_blank">
      <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
        <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/>
        <rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/>
      </svg>
      LinkedIn
    </a>
  </div>

  <footer>
    <p>Soaeb Abdullah · Software Engineer</p>
    <p>Dhaka, Bangladesh <span class="flag">🇧🇩</span></p>
  </footer>

</div>
</body>
</html>
