[![MasterHead](https://www.vackergroup.ae/wp-content/uploads/2016/04/Iot-cover-image.gif)](https://www.linkedin.com/in/soaeb-abdullah/)

<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Soaeb Abdullah — GitHub Banner</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=Fraunces:ital,opsz,wght@0,9..144,300;0,9..144,600;1,9..144,300&display=swap" rel="stylesheet"/>
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    background: #070809;
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    font-family: 'DM Mono', monospace;
  }

  .banner {
    width: 1200px;
    height: 400px;
    background: #0e0f11;
    position: relative;
    overflow: hidden;
    border-left: 4px solid #1D9E75;
  }

  /* Grid lines */
  .grid {
    position: absolute;
    inset: 0;
    background-image:
      linear-gradient(rgba(255,255,255,0.035) 1px, transparent 1px),
      linear-gradient(90deg, rgba(255,255,255,0.035) 1px, transparent 1px);
    background-size: 80px 80px;
  }

  /* Right edge glow accent */
  .banner::after {
    content: '';
    position: absolute;
    top: 0; right: 0;
    width: 3px; height: 100%;
    background: linear-gradient(180deg, transparent, #1D9E75 50%, transparent);
    opacity: 0.3;
  }

  /* ── LEFT SIDE ── */
  .left {
    position: absolute;
    left: 48px;
    top: 50%;
    transform: translateY(-50%);
    display: flex;
    align-items: center;
    gap: 40px;
  }

  /* Avatar */
  .avatar {
    width: 130px;
    height: 130px;
    border-radius: 50%;
    border: 1.5px solid #1D9E75;
    background: #1a2420;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'Fraunces', serif;
    font-size: 42px;
    font-weight: 600;
    color: #1D9E75;
    flex-shrink: 0;
    position: relative;
    animation: avatarIn 0.8s cubic-bezier(0.16,1,0.3,1) both;
  }

  .avatar::after {
    content: '';
    position: absolute;
    bottom: 6px; right: 6px;
    width: 14px; height: 14px;
    border-radius: 50%;
    background: #1D9E75;
    border: 2.5px solid #0e0f11;
    animation: pulse 2.5s infinite;
  }

  @keyframes pulse {
    0%, 100% { transform: scale(1); opacity: 1; }
    50% { transform: scale(0.85); opacity: 0.5; }
  }

  /* Name block */
  .name-block {
    animation: slideIn 0.7s 0.1s cubic-bezier(0.16,1,0.3,1) both;
  }

  .name-row {
    display: flex;
    align-items: baseline;
    gap: 16px;
    line-height: 1;
  }

  .name-first {
    font-family: 'Fraunces', serif;
    font-size: 64px;
    font-weight: 600;
    color: #e8e6e1;
    letter-spacing: -2px;
  }

  .name-last {
    font-family: 'Fraunces', serif;
    font-size: 64px;
    font-weight: 300;
    font-style: italic;
    color: #1D9E75;
    letter-spacing: -2px;
  }

  .role-row {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-top: 12px;
  }

  .role-line {
    width: 28px;
    height: 1px;
    background: #1D9E75;
  }

  .role-text {
    font-size: 12px;
    color: #7a7875;
    letter-spacing: 0.2em;
    text-transform: uppercase;
  }

  /* Tags row */
  .tags {
    display: flex;
    gap: 8px;
    margin-top: 20px;
    animation: slideIn 0.7s 0.2s cubic-bezier(0.16,1,0.3,1) both;
  }

  .tag {
    font-size: 11px;
    padding: 5px 13px;
    border-radius: 5px;
    font-family: 'DM Mono', monospace;
    letter-spacing: 0.03em;
  }

  .tag-green  { background: #0f2e24; border: 1px solid rgba(29,158,117,0.45); color: #5DCAA5; }
  .tag-amber  { background: #2a1f08; border: 1px solid rgba(239,159,39,0.4);  color: #EF9F27; }
  .tag-purple { background: #1a1728; border: 1px solid rgba(175,169,236,0.4); color: #AFA9EC; }
  .tag-gray   { background: #161719; border: 1px solid rgba(255,255,255,0.1); color: #888780; }

  /* Links */
  .links {
    margin-top: 18px;
    display: flex;
    flex-direction: column;
    gap: 4px;
    animation: slideIn 0.7s 0.3s cubic-bezier(0.16,1,0.3,1) both;
  }

  .link-item {
    font-size: 11px;
    color: #5a5856;
    letter-spacing: 0.04em;
    display: flex;
    align-items: center;
    gap: 6px;
  }

  .link-dot {
    width: 4px; height: 4px;
    border-radius: 50%;
    background: #1D9E75;
    opacity: 0.6;
    flex-shrink: 0;
  }

  /* ── RIGHT SIDE — Code Panel ── */
  .code-panel {
    position: absolute;
    right: 48px;
    top: 36px;
    width: 420px;
    height: 328px;
    background: #161719;
    border: 1px solid rgba(255,255,255,0.07);
    border-radius: 10px;
    overflow: hidden;
    animation: panelIn 0.8s 0.15s cubic-bezier(0.16,1,0.3,1) both;
  }

  .code-panel::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 2px;
    background: #1D9E75;
    opacity: 0.9;
  }

  .panel-header {
    display: flex;
    align-items: center;
    gap: 7px;
    padding: 16px 18px 12px;
    border-bottom: 1px solid rgba(255,255,255,0.05);
  }

  .dot { width: 10px; height: 10px; border-radius: 50%; }
  .dot-r { background: #ff5f56; }
  .dot-y { background: #ffbd2e; }
  .dot-g { background: #27c93f; }

  .panel-filename {
    margin-left: auto;
    font-size: 11px;
    color: #5a5856;
    letter-spacing: 0.04em;
  }

  .code-body {
    padding: 16px 18px;
    font-size: 13px;
    line-height: 2.1;
  }

  .code-line { display: flex; gap: 16px; }
  .ln { color: #333; min-width: 16px; text-align: right; user-select: none; }
  .code-kw   { color: #AFA9EC; }
  .code-fn   { color: #5DCAA5; }
  .code-str  { color: #FAC775; }
  .code-cm   { color: #555452; font-style: italic; }
  .code-op   { color: #555452; }
  .code-txt  { color: #e8e6e1; }

  .cursor {
    display: inline-block;
    width: 8px; height: 14px;
    background: #1D9E75;
    vertical-align: middle;
    margin-left: 2px;
    border-radius: 1px;
    animation: blink 1.1s step-end infinite;
  }

  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }

  .panel-footer {
    position: absolute;
    bottom: 0; left: 0; right: 0;
    background: rgba(10,11,12,0.7);
    padding: 7px 18px;
    display: flex;
    align-items: center;
    gap: 8px;
    border-top: 1px solid rgba(255,255,255,0.04);
  }

  .branch-dot { width: 7px; height: 7px; border-radius: 50%; background: #1D9E75; }
  .branch-name { font-size: 11px; color: #5a5856; }
  .py-label { margin-left: auto; font-size: 11px; color: #5a5856; }

  /* Animations */
  @keyframes avatarIn {
    from { opacity: 0; transform: scale(0.85); }
    to   { opacity: 1; transform: scale(1); }
  }
  @keyframes slideIn {
    from { opacity: 0; transform: translateX(-20px); }
    to   { opacity: 1; transform: translateX(0); }
  }
  @keyframes panelIn {
    from { opacity: 0; transform: translateY(20px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  /* Decorative floating dots top-right */
  .deco {
    position: absolute;
    top: 28px; right: 490px;
    display: flex;
    gap: 10px;
    opacity: 0.35;
  }
  .deco span {
    width: 5px; height: 5px;
    border-radius: 50%;
    background: #1D9E75;
  }
  .deco span:nth-child(2) { opacity: 0.6; }
  .deco span:nth-child(3) { opacity: 0.3; }
</style>
</head>
<body>

<div class="banner">
  <div class="grid"></div>
  <div class="deco"><span></span><span></span><span></span></div>

  <!-- LEFT -->
  <div class="left">
    <div class="avatar">SA</div>

    <div>
      <div class="name-block">
        <div class="name-row">
          <span class="name-first">Soaeb</span>
          <span class="name-last">Abdullah</span>
        </div>
        <div class="role-row">
          <span class="role-line"></span>
          <span class="role-text">Software Engineer &nbsp;·&nbsp; Bangladesh</span>
        </div>
      </div>

      <div class="tags">
        <span class="tag tag-green">Odoo Dev</span>
        <span class="tag tag-amber">DevOps</span>
        <span class="tag tag-purple">Tech PM</span>
        <span class="tag tag-gray">🇧🇩 BD</span>
      </div>

      <div class="links">
        <span class="link-item"><span class="link-dot"></span>linkedin.com/in/soaeb-abdullah</span>
        <span class="link-item"><span class="link-dot"></span>availabilityshare.com</span>
      </div>
    </div>
  </div>

  <!-- RIGHT code panel -->
  <div class="code-panel">
    <div class="panel-header">
      <span class="dot dot-r"></span>
      <span class="dot dot-y"></span>
      <span class="dot dot-g"></span>
      <span class="panel-filename">about.py</span>
    </div>

    <div class="code-body">
      <div class="code-line"><span class="ln">1</span><span><span class="code-kw">class </span><span class="code-fn">Soaeb</span><span class="code-op">(</span><span class="code-fn">Engineer</span><span class="code-op">):</span></span></div>
      <div class="code-line"><span class="ln">2</span><span class="code-cm">&nbsp;&nbsp;# Dhaka, Bangladesh 🇧🇩</span></div>
      <div class="code-line"><span class="ln">3</span><span><span class="code-txt">&nbsp;&nbsp;stack &nbsp;&nbsp;&nbsp;</span><span class="code-op">= </span><span class="code-str">"Odoo · Python"</span></span></div>
      <div class="code-line"><span class="ln">4</span><span><span class="code-txt">&nbsp;&nbsp;infra &nbsp;&nbsp;&nbsp;</span><span class="code-op">= </span><span class="code-str">"Docker · Nginx · AWS"</span></span></div>
      <div class="code-line"><span class="ln">5</span><span><span class="code-txt">&nbsp;&nbsp;db &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="code-op">= </span><span class="code-str">"PostgreSQL · MySQL"</span></span></div>
      <div class="code-line"><span class="ln">6</span><span><span class="code-txt">&nbsp;&nbsp;building </span><span class="code-op">= </span><span class="code-str">"availabilityshare.com"</span></span></div>
      <div class="code-line"><span class="ln">7</span><span>&nbsp;&nbsp;<span class="cursor"></span></span></div>
    </div>

    <div class="panel-footer">
      <span class="branch-dot"></span>
      <span class="branch-name">main</span>
      <span class="py-label">Python 3.11</span>
    </div>
  </div>

</div>


<h1 align="center">Hi 👋, I'm Soaeb Abdullah</h1>
<h3 align="center">A passionate Software Engineer from Bangladesh</h3>
<p class="hero-sub">
        Odoo Developer &amp; DevOps Engineer. Building scalable ERP solutions and shipping production infrastructure from Dhaka.
      </p>
<img  align="right" alt="Coding" width="400" src="https://gifdb.com/images/high/animated-man-computer-coding-nae6mec378lsg1i3.webp">

- 🔭 I’m currently working on [Availability share](https://www.availabilityshare.com/)

- 🌱 I’m currently learning **Odoo**

- 👨‍💻 All of my projects are available at [https://www.linkedin.com/in/soaeb-abdullah/](https://www.linkedin.com/in/soaeb-abdullah/)

- 📄 Know about my experiences [https://drive.google.com/file/d/1E0YmnXrqEETQbu_dkPykk_IkA4HQPURg/view?usp=sharing](https://drive.google.com/file/d/1E0YmnXrqEETQbu_dkPykk_IkA4HQPURg/view?usp=sharing)

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://linkedin.com/in/https://www.linkedin.com/in/soaeb-abdullah/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="https://www.linkedin.com/in/soaeb-abdullah/" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://developer.android.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/android/android-original-wordmark.svg" alt="android" width="40" height="40"/> </a> <a href="https://www.arduino.cc/" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/arduino-1.svg" alt="arduino" width="40" height="40"/> </a> <a href="https://aws.amazon.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"/> </a> <a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a> <a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cpp/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cs/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg" alt="csharp" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.docker.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> </a> <a href="https://www.figma.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" alt="figma" width="40" height="40"/> </a> <a href="https://firebase.google.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" alt="firebase" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://www.adobe.com/in/products/illustrator.html" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/adobe_illustrator/adobe_illustrator-icon.svg" alt="illustrator" width="40" height="40"/> </a> <a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://www.nginx.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nginx/nginx-original.svg" alt="nginx" width="40" height="40"/> </a> <a href="https://opencv.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/opencv/opencv-icon.svg" alt="opencv" width="40" height="40"/> </a> <a href="https://www.postgresql.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/> </a> <a href="https://postman.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" alt="postman" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://www.sketch.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/sketchapp/sketchapp-icon.svg" alt="sketch" width="40" height="40"/> </a> </p>
