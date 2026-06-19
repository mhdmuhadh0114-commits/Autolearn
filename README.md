<WELCOME OUR AUTOMOBILE LEARNING SITE>
<html lang="ta-LK" dir="ltr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AutoMaster Tamil – Automobile Learning & NVQ Level 3</title>
  <meta name="description" content="AutoMaster Tamil – Learn automobile engineering in Tamil. Engine systems, NVQ Level 3 study materials, MCQ quizzes and more." />
  <meta name="keywords" content="automobile Tamil, NVQ Level 3, engine systems, automotive engineering Tamil, MCQ quiz" />
  <meta property="og:title" content="AutoMaster Tamil" />
  <meta property="og:description" content="Automobile learning in Tamil – NVQ Level 3 study materials, engine notes & MCQ quizzes." />
  <meta name="theme-color" content="#e85d04" />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@400;600;700;900&family=Noto+Sans+Tamil:wght@400;600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet" />
  <style>
    /* ── TOKENS ─────────────────────────────────────────────── */
    :root {
      --bg:        #0d0d0f;
      --surface:   #161618;
      --surface2:  #1e1e21;
      --border:    #2a2a2f;
      --accent:    #e85d04;
      --accent2:   #ff9f1c;
      --text:      #f0ede8;
      --muted:     #8a8790;
      --success:   #22c55e;
      --danger:    #ef4444;
      --font-head: 'Barlow Condensed', sans-serif;
      --font-tamil:'Noto Sans Tamil', sans-serif;
      --font-body: 'Inter', sans-serif;
      --radius:    8px;
      --glow: 0 0 32px rgba(232,93,4,.25);
    }
    [data-theme="light"] {
      --bg:       #f5f3ef;
      --surface:  #ffffff;
      --surface2: #ede9e3;
      --border:   #d6d0c8;
      --text:     #1a1814;
      --muted:    #6b6560;
      --glow: 0 0 32px rgba(232,93,4,.15);
    }

    /* ── RESET ───────────────────────────────────────────────── */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body {
      font-family: var(--font-body);
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
      transition: background .3s, color .3s;
      overflow-x: hidden;
    }
    img { max-width: 100%; display: block; }
    a { color: inherit; text-decoration: none; }
    button { cursor: pointer; font-family: inherit; }

    /* ── NAV ─────────────────────────────────────────────────── */
    nav {
      position: fixed; top: 0; width: 100%; z-index: 100;
      background: rgba(13,13,15,.88);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--border);
      padding: 0 1.5rem;
      display: flex; align-items: center; justify-content: space-between;
      height: 62px;
      transition: background .3s;
    }
    [data-theme="light"] nav { background: rgba(245,243,239,.9); }
    .nav-logo {
      font-family: var(--font-head);
      font-size: 1.6rem; font-weight: 900; letter-spacing: .02em;
      color: var(--text);
    }
    .nav-logo span { color: var(--accent); }
    .nav-links { display: flex; gap: 1.6rem; align-items: center; }
    .nav-links a {
      font-size: .88rem; font-weight: 500; color: var(--muted);
      transition: color .2s;
    }
    .nav-links a:hover, .nav-links a.active { color: var(--accent); }
    .nav-right { display: flex; gap: .75rem; align-items: center; }
    .btn-theme {
      background: var(--surface2); border: 1px solid var(--border);
      border-radius: 50%; width: 36px; height: 36px;
      display: grid; place-items: center; font-size: 1rem;
      transition: background .2s;
    }
    .btn-theme:hover { background: var(--accent); }
    .hamburger {
      display: none; flex-direction: column; gap: 5px;
      background: none; border: none; padding: 4px;
    }
    .hamburger span {
      display: block; width: 22px; height: 2px;
      background: var(--text); border-radius: 2px;
      transition: all .3s;
    }
    .mobile-menu {
      display: none; position: fixed; top: 62px; left: 0; right: 0;
      background: var(--surface); border-bottom: 1px solid var(--border);
      padding: 1rem 1.5rem; z-index: 99;
    }
    .mobile-menu.open { display: block; }
    .mobile-menu a {
      display: block; padding: .65rem 0;
      border-bottom: 1px solid var(--border);
      color: var(--muted); font-size: .95rem;
    }
    .mobile-menu a:last-child { border-bottom: none; }

    /* ── HERO ─────────────────────────────────────────────────── */
    #home {
      min-height: 100vh;
      display: flex; align-items: center; justify-content: center;
      position: relative; overflow: hidden;
      padding: 80px 1.5rem 3rem;
    }
    .hero-bg {
      position: absolute; inset: 0; z-index: 0;
      background: radial-gradient(ellipse 80% 60% at 50% 30%, rgba(232,93,4,.18) 0%, transparent 70%),
                  radial-gradient(ellipse 50% 40% at 80% 70%, rgba(255,159,28,.1) 0%, transparent 60%);
    }
    /* animated engine grid */
    .hero-grid {
      position: absolute; inset: 0; z-index: 0; opacity: .06;
      background-image:
        linear-gradient(var(--border) 1px, transparent 1px),
        linear-gradient(90deg, var(--border) 1px, transparent 1px);
      background-size: 40px 40px;
    }
    .hero-content { position: relative; z-index: 1; text-align: center; max-width: 820px; }
    .hero-badge {
      display: inline-flex; align-items: center; gap: .5rem;
      background: rgba(232,93,4,.15); border: 1px solid rgba(232,93,4,.35);
      border-radius: 50px; padding: .35rem 1rem;
      font-size: .78rem; font-weight: 600; color: var(--accent2);
      letter-spacing: .06em; text-transform: uppercase; margin-bottom: 1.5rem;
    }
    .hero-badge::before { content: '⚙️'; font-size: .9rem; }
    .hero-title {
      font-family: var(--font-head);
      font-size: clamp(3rem, 9vw, 7rem);
      font-weight: 900; line-height: .95; letter-spacing: -.01em;
      text-transform: uppercase; margin-bottom: .5rem;
    }
    .hero-title .accent { color: var(--accent); display: block; }
    .hero-tamil {
      font-family: var(--font-tamil);
      font-size: clamp(1.2rem, 3vw, 1.7rem);
      color: var(--muted); margin-bottom: 1.8rem; font-weight: 400;
    }
    .hero-desc {
      font-size: 1rem; color: var(--muted); max-width: 560px;
      margin: 0 auto 2.5rem; line-height: 1.7;
    }
    .hero-cta { display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap; }
    .btn-primary {
      background: var(--accent); color: #fff;
      padding: .75rem 1.8rem; border-radius: var(--radius);
      font-size: .95rem; font-weight: 600; border: none;
      box-shadow: var(--glow); transition: transform .2s, box-shadow .2s;
    }
    .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 0 48px rgba(232,93,4,.4); }
    .btn-outline {
      background: transparent; color: var(--text);
      padding: .75rem 1.8rem; border-radius: var(--radius);
      font-size: .95rem; font-weight: 600;
      border: 1px solid var(--border);
      transition: border-color .2s, color .2s;
    }
    .btn-outline:hover { border-color: var(--accent); color: var(--accent); }
    .hero-stats {
      display: flex; gap: 2.5rem; justify-content: center;
      flex-wrap: wrap; margin-top: 3.5rem;
    }
    .stat { text-align: center; }
    .stat-num {
      font-family: var(--font-head);
      font-size: 2.2rem; font-weight: 900; color: var(--accent);
      line-height: 1;
    }
    .stat-label { font-size: .78rem; color: var(--muted); letter-spacing: .05em; margin-top: .2rem; }

    /* ── SECTION BASE ─────────────────────────────────────────── */
    section { padding: 5rem 1.5rem; }
    .section-inner { max-width: 1100px; margin: 0 auto; }
    .section-label {
      font-size: .72rem; font-weight: 700; letter-spacing: .12em;
      text-transform: uppercase; color: var(--accent);
      margin-bottom: .75rem;
    }
    .section-title {
      font-family: var(--font-head);
      font-size: clamp(2rem, 4vw, 3rem);
      font-weight: 800; letter-spacing: -.01em; line-height: 1.1;
      margin-bottom: 1rem;
    }
    .section-sub { color: var(--muted); max-width: 580px; line-height: 1.7; }

    /* ── LEARNING SECTION ────────────────────────────────────── */
    #learning { background: var(--surface); }
    .learn-grid {
      display: grid; gap: 1.25rem;
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
      margin-top: 2.5rem;
    }
    .learn-card {
      background: var(--bg); border: 1px solid var(--border);
      border-radius: var(--radius); padding: 1.5rem;
      transition: border-color .25s, transform .25s, box-shadow .25s;
      cursor: pointer;
    }
    .learn-card:hover {
      border-color: var(--accent);
      transform: translateY(-4px);
      box-shadow: var(--glow);
    }
    .learn-icon {
      width: 48px; height: 48px; border-radius: 10px;
      background: rgba(232,93,4,.12);
      display: grid; place-items: center;
      font-size: 1.5rem; margin-bottom: 1rem;
    }
    .learn-card h3 {
      font-family: var(--font-head); font-size: 1.25rem;
      font-weight: 700; margin-bottom: .4rem;
    }
    .learn-card .tamil-sub {
      font-family: var(--font-tamil); font-size: .82rem; color: var(--muted); margin-bottom: .8rem;
    }
    .learn-card p { font-size: .88rem; color: var(--muted); line-height: 1.6; }

    /* ── ENGINE NOTES ─────────────────────────────────────────── */
    #engine { background: var(--bg); }
    .accordion { margin-top: 2.5rem; display: flex; flex-direction: column; gap: .75rem; }
    .acc-item {
      background: var(--surface); border: 1px solid var(--border);
      border-radius: var(--radius); overflow: hidden;
    }
    .acc-head {
      display: flex; align-items: center; justify-content: space-between;
      padding: 1rem 1.25rem; background: none; border: none;
      width: 100%; text-align: left; color: var(--text);
      font-family: var(--font-head); font-size: 1.1rem; font-weight: 700;
      letter-spacing: .02em; cursor: pointer; gap: 1rem;
    }
    .acc-head:hover { color: var(--accent); }
    .acc-arrow {
      font-size: 1.2rem; transition: transform .3s; flex-shrink: 0; color: var(--accent);
    }
    .acc-item.open .acc-arrow { transform: rotate(180deg); }
    .acc-body {
      max-height: 0; overflow: hidden;
      transition: max-height .4s cubic-bezier(.4,0,.2,1), padding .3s;
      padding: 0 1.25rem;
    }
    .acc-item.open .acc-body { max-height: 900px; padding: 0 1.25rem 1.25rem; }
    .acc-body p {
      color: var(--muted); font-size: .9rem; line-height: 1.7;
      border-top: 1px solid var(--border); padding-top: 1rem;
    }
    .acc-body ul { list-style: none; margin-top: .75rem; }
    .acc-body ul li {
      position: relative; padding-left: 1.25rem;
      color: var(--muted); font-size: .88rem; line-height: 1.7;
    }
    .acc-body ul li::before {
      content: '›'; position: absolute; left: 0;
      color: var(--accent); font-weight: 700;
    }
    .acc-body .note-tag {
      display: inline-block; margin-top: .75rem;
      font-size: .72rem; background: rgba(232,93,4,.12);
      color: var(--accent2); border-radius: 4px; padding: .2rem .5rem; font-weight: 600;
    }

    /* ── NVQ SECTION ──────────────────────────────────────────── */
    #nvq { background: var(--surface); }
    .nvq-grid {
      display: grid; gap: 1.25rem;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      margin-top: 2.5rem;
    }
    .nvq-card {
      background: var(--bg); border: 1px solid var(--border);
      border-radius: var(--radius); overflow: hidden;
      transition: border-color .25s, transform .25s;
    }
    .nvq-card:hover { border-color: var(--accent); transform: translateY(-3px); }
    .nvq-card-head {
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      padding: 1.25rem; color: #fff;
    }
    .nvq-card-head .unit-code {
      font-size: .72rem; font-weight: 700; letter-spacing: .1em;
      opacity: .8; margin-bottom: .3rem;
    }
    .nvq-card-head h3 {
      font-family: var(--font-head); font-size: 1.15rem; font-weight: 800;
    }
    .nvq-card-head .tamil {
      font-family: var(--font-tamil); font-size: .8rem; opacity: .85; margin-top: .2rem;
    }
    .nvq-card-body { padding: 1.25rem; }
    .nvq-card-body p { font-size: .87rem; color: var(--muted); line-height: 1.6; }
    .nvq-topics { margin-top: .85rem; display: flex; flex-wrap: wrap; gap: .4rem; }
    .nvq-topics span {
      font-size: .72rem; background: var(--surface2);
      border: 1px solid var(--border); border-radius: 4px;
      padding: .2rem .55rem; color: var(--muted);
    }
    .nvq-progress { margin-top: 1rem; }
    .progress-label {
      display: flex; justify-content: space-between;
      font-size: .75rem; color: var(--muted); margin-bottom: .4rem;
    }
    .progress-bar {
      height: 4px; background: var(--border); border-radius: 2px; overflow: hidden;
    }
    .progress-fill {
      height: 100%; background: linear-gradient(90deg, var(--accent), var(--accent2));
      border-radius: 2px; transition: width .8s ease;
    }

    /* ── MCQ QUIZ ──────────────────────────────────────────────── */
    #quiz { background: var(--bg); }
    .quiz-wrapper {
      max-width: 680px; margin: 2.5rem auto 0;
      background: var(--surface); border: 1px solid var(--border);
      border-radius: 12px; overflow: hidden;
    }
    .quiz-header {
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      padding: 1.5rem; color: #fff;
    }
    .quiz-header h3 {
      font-family: var(--font-head); font-size: 1.4rem; font-weight: 800;
    }
    .quiz-header p { opacity: .85; font-size: .88rem; margin-top: .25rem; }
    .quiz-meta {
      display: flex; gap: 1.5rem; margin-top: 1rem;
    }
    .quiz-meta span { font-size: .8rem; opacity: .9; }
    .quiz-meta b { font-weight: 700; }
    .quiz-body { padding: 1.75rem; }
    .quiz-category-tabs {
      display: flex; gap: .5rem; flex-wrap: wrap; margin-bottom: 1.5rem;
    }
    .quiz-tab {
      padding: .4rem .9rem; border-radius: 50px;
      font-size: .8rem; font-weight: 600;
      background: var(--surface2); border: 1px solid var(--border);
      color: var(--muted); transition: all .2s;
    }
    .quiz-tab.active, .quiz-tab:hover {
      background: var(--accent); border-color: var(--accent); color: #fff;
    }
    .question-num {
      font-size: .78rem; color: var(--muted); margin-bottom: .5rem; font-weight: 600;
    }
    .question-text {
      font-size: 1.05rem; font-weight: 600; margin-bottom: 1.25rem; line-height: 1.5;
    }
    .question-tamil {
      font-family: var(--font-tamil); font-size: .9rem;
      color: var(--muted); margin-bottom: 1.25rem; margin-top: -.75rem;
    }
    .options { display: flex; flex-direction: column; gap: .65rem; }
    .opt-btn {
      background: var(--surface2); border: 1.5px solid var(--border);
      border-radius: var(--radius); padding: .85rem 1rem;
      text-align: left; font-size: .92rem; color: var(--text);
      transition: all .2s; display: flex; align-items: center; gap: .75rem;
    }
    .opt-btn:hover:not(:disabled) {
      border-color: var(--accent); background: rgba(232,93,4,.08);
    }
    .opt-btn.correct { border-color: var(--success); background: rgba(34,197,94,.12); color: var(--success); }
    .opt-btn.wrong   { border-color: var(--danger);  background: rgba(239,68,68,.12);  color: var(--danger); }
    .opt-btn .opt-letter {
      width: 28px; height: 28px; border-radius: 50%;
      background: var(--border); display: grid; place-items: center;
      font-size: .78rem; font-weight: 700; flex-shrink: 0;
      transition: background .2s, color .2s;
    }
    .opt-btn.correct .opt-letter { background: var(--success); color: #fff; }
    .opt-btn.wrong   .opt-letter { background: var(--danger);  color: #fff; }
    .quiz-feedback {
      margin-top: 1rem; padding: .85rem 1rem;
      border-radius: var(--radius); font-size: .9rem; line-height: 1.5;
      display: none;
    }
    .quiz-feedback.show { display: block; }
    .quiz-feedback.correct-fb {
      background: rgba(34,197,94,.12); border: 1px solid rgba(34,197,94,.3); color: var(--success);
    }
    .quiz-feedback.wrong-fb {
      background: rgba(239,68,68,.1); border: 1px solid rgba(239,68,68,.25); color: var(--danger);
    }
    .quiz-nav {
      display: flex; justify-content: space-between; align-items: center;
      margin-top: 1.5rem; flex-wrap: wrap; gap: .75rem;
    }
    .quiz-score-badge {
      font-family: var(--font-head); font-size: 1rem; font-weight: 700;
      color: var(--accent);
    }
    .quiz-progress-bar {
      height: 3px; background: var(--border); margin-top: 1.5rem; border-radius: 2px;
    }
    .quiz-progress-fill {
      height: 100%; background: linear-gradient(90deg, var(--accent), var(--accent2));
      border-radius: 2px; transition: width .4s ease;
    }
    .quiz-result {
      text-align: center; padding: 2rem 1.75rem; display: none;
    }
    .quiz-result.show { display: block; }
    .result-score {
      font-family: var(--font-head); font-size: 4rem; font-weight: 900; color: var(--accent);
    }
    .result-label { font-size: 1.1rem; color: var(--muted); margin-bottom: 1.5rem; }

    /* ── CONTACT ──────────────────────────────────────────────── */
    #contact { background: var(--surface); }
    .contact-grid {
      display: grid; gap: 3rem;
      grid-template-columns: 1fr 1.4fr;
      margin-top: 2.5rem;
    }
    .contact-info h3 {
      font-family: var(--font-head); font-size: 1.5rem; font-weight: 800; margin-bottom: 1rem;
    }
    .contact-info p { color: var(--muted); font-size: .9rem; line-height: 1.7; margin-bottom: 1.5rem; }
    .contact-item {
      display: flex; gap: .75rem; align-items: flex-start;
      padding: .85rem 0; border-bottom: 1px solid var(--border);
    }
    .contact-item:last-of-type { border-bottom: none; }
    .contact-ico {
      width: 36px; height: 36px; border-radius: 8px;
      background: rgba(232,93,4,.12); display: grid; place-items: center;
      font-size: 1rem; flex-shrink: 0;
    }
    .contact-item-text strong { display: block; font-size: .88rem; font-weight: 600; }
    .contact-item-text span { font-size: .82rem; color: var(--muted); }
    .contact-form { display: flex; flex-direction: column; gap: 1rem; }
    .form-row { display: grid; gap: 1rem; grid-template-columns: 1fr 1fr; }
    .form-field { display: flex; flex-direction: column; gap: .4rem; }
    .form-field label { font-size: .8rem; font-weight: 600; color: var(--muted); }
    .form-field input, .form-field textarea, .form-field select {
      background: var(--bg); border: 1.5px solid var(--border);
      border-radius: var(--radius); padding: .75rem 1rem;
      color: var(--text); font-size: .9rem; font-family: var(--font-body);
      transition: border-color .2s;
      outline: none;
    }
    .form-field input:focus, .form-field textarea:focus, .form-field select:focus {
      border-color: var(--accent);
    }
    .form-field textarea { resize: vertical; min-height: 110px; }
    .form-success {
      display: none; background: rgba(34,197,94,.12);
      border: 1px solid rgba(34,197,94,.3); border-radius: var(--radius);
      padding: 1rem; color: var(--success); text-align: center; font-size: .9rem;
    }
    .form-success.show { display: block; }

    /* ── FOOTER ──────────────────────────────────────────────── */
    footer {
      background: var(--bg); border-top: 1px solid var(--border);
      padding: 2.5rem 1.5rem; text-align: center;
    }
    .footer-logo {
      font-family: var(--font-head); font-size: 1.5rem; font-weight: 900;
      margin-bottom: .5rem;
    }
    .footer-logo span { color: var(--accent); }
    footer p { color: var(--muted); font-size: .82rem; }
    .footer-links { display: flex; gap: 1.5rem; justify-content: center; flex-wrap: wrap; margin: 1rem 0; }
    .footer-links a { color: var(--muted); font-size: .82rem; transition: color .2s; }
    .footer-links a:hover { color: var(--accent); }

    /* ── SCROLL TO TOP ───────────────────────────────────────── */
    #scrollTop {
      position: fixed; bottom: 1.5rem; right: 1.5rem; z-index: 90;
      background: var(--accent); color: #fff;
      width: 42px; height: 42px; border-radius: 50%; border: none;
      font-size: 1.1rem; display: grid; place-items: center;
      box-shadow: var(--glow); opacity: 0; pointer-events: none;
      transition: opacity .3s, transform .3s;
    }
    #scrollTop.visible { opacity: 1; pointer-events: auto; }
    #scrollTop:hover { transform: translateY(-3px); }

    /* ── RESPONSIVE ──────────────────────────────────────────── */
    @media (max-width: 768px) {
      .nav-links { display: none; }
      .hamburger { display: flex; }
      .contact-grid { grid-template-columns: 1fr; }
      .form-row { grid-template-columns: 1fr; }
      .hero-stats { gap: 1.5rem; }
    }
    @media (max-width: 480px) {
      .learn-grid, .nvq-grid { grid-template-columns: 1fr; }
    }
    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after { transition-duration: .01ms !important; animation-duration: .01ms !important; }
    }

    /* ── PISTON ANIMATION ────────────────────────────────────── */
    .piston-svg {
      margin: 2rem auto 0; display: block; opacity: .18;
    }
  </style>
</head>
<body>

<!-- NAV -->
<nav id="navbar">
  <a class="nav-logo" href="#home">Auto<span>Master</span> Tamil</a>
  <ul class="nav-links" role="list">
    <li><a href="#home" class="active">Home</a></li>
    <li><a href="#learning">Learning</a></li>
    <li><a href="#engine">Engine Notes</a></li>
    <li><a href="#nvq">NVQ Level 3</a></li>
    <li><a href="#quiz">MCQ Quiz</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
  <div class="nav-right">
    <button class="btn-theme" id="themeToggle" aria-label="Toggle dark/light mode">🌙</button>
    <button class="hamburger" id="hamburger" aria-label="Open menu" aria-expanded="false">
      <span></span><span></span><span></span>
    </button>
  </div>
</nav>

<!-- MOBILE MENU -->
<div class="mobile-menu" id="mobileMenu" role="navigation">
  <a href="#home">🏠 Home</a>
  <a href="#learning">📚 Learning</a>
  <a href="#engine">⚙️ Engine Notes</a>
  <a href="#nvq">🎓 NVQ Level 3</a>
  <a href="#quiz">❓ MCQ Quiz</a>
  <a href="#contact">📞 Contact</a>
</div>

<!-- HERO -->
<section id="home">
  <div class="hero-bg"></div>
  <div class="hero-grid"></div>
  <div class="hero-content">
    <div class="hero-badge">Sri Lanka's Automotive Tamil Platform</div>
    <h1 class="hero-title">
      Auto<span class="accent">Master</span>
    </h1>
    <p class="hero-tamil">தமிழில் ஆட்டோமொபைல் கற்றல் தளம்</p>
    <p class="hero-desc">
      Learn automobile engineering in Tamil — engine systems, NVQ Level 3 study materials,
      and MCQ quizzes designed for aspiring automotive technicians.
    </p>
    <div class="hero-cta">
      <button class="btn-primary" onclick="document.querySelector('#learning').scrollIntoView({behavior:'smooth'})">Start Learning</button>
      <button class="btn-outline" onclick="document.querySelector('#quiz').scrollIntoView({behavior:'smooth'})">Take MCQ Quiz</button>
    </div>
    <div class="hero-stats">
      <div class="stat">
        <div class="stat-num">50+</div>
        <div class="stat-label">Tamil Notes</div>
      </div>
      <div class="stat">
        <div class="stat-num">200+</div>
        <div class="stat-label">MCQ Questions</div>
      </div>
      <div class="stat">
        <div class="stat-num">NVQ3</div>
        <div class="stat-label">Level 3 Content</div>
      </div>
      <div class="stat">
        <div class="stat-num">Free</div>
        <div class="stat-label">Always Free</div>
      </div>
    </div>
  </div>
</section>

<!-- LEARNING -->
<section id="learning">
  <div class="section-inner">
    <p class="section-label">Automobile Learning</p>
    <h2 class="section-title">Explore Every System<br>ஒவ்வொரு அமைப்பையும் கற்றுக்கொள்</h2>
    <p class="section-sub">Structured modules covering all key automobile systems — from engine fundamentals to advanced diagnostics, explained clearly in Tamil.</p>
    <div class="learn-grid" id="learnGrid"></div>
  </div>
</section>

<!-- ENGINE NOTES -->
<section id="engine">
  <div class="section-inner">
    <p class="section-label">Engine Systems Notes</p>
    <h2 class="section-title">Engine System Deep Dives<br>என்ஜின் அமைப்பு விளக்கங்கள்</h2>
    <p class="section-sub">Comprehensive notes on each engine sub-system — tap any topic to expand the full explanation.</p>
    <div class="accordion" id="accordion"></div>
  </div>
</section>

<!-- NVQ LEVEL 3 -->
<section id="nvq">
  <div class="section-inner">
    <p class="section-label">NVQ Level 3 Study Materials</p>
    <h2 class="section-title">NVQ Level 3 Units<br>NVQ நிலை 3 அலகுகள்</h2>
    <p class="section-sub">Official unit materials mapped to TVEC Sri Lanka NVQ Level 3 Light Vehicle Technology competencies.</p>
    <div class="nvq-grid" id="nvqGrid"></div>
  </div>
</section>

<!-- MCQ QUIZ -->
<section id="quiz">
  <div class="section-inner">
    <p class="section-label">MCQ Quiz</p>
    <h2 class="section-title">Test Your Knowledge<br>உங்கள் அறிவை சோதிக்கவும்</h2>
    <p class="section-sub">Practice MCQs with instant feedback — perfect for NVQ exam preparation.</p>

    <div class="quiz-wrapper">
      <div class="quiz-header">
        <h3>⚙️ AutoMaster MCQ Quiz</h3>
        <p>Select a category and answer all questions</p>
        <div class="quiz-meta">
          <span>Category: <b id="quizCatLabel">Engine</b></span>
          <span>Question: <b id="qNum">1</b>/<b id="qTotal">5</b></span>
          <span>Score: <b id="scoreLive">0</b></span>
        </div>
      </div>
      <div class="quiz-body" id="quizBody">
        <div class="quiz-category-tabs" id="catTabs"></div>
        <div id="quizQuestion">
          <div class="question-num" id="questionNum">Question 1 of 5</div>
          <div class="question-text" id="questionText"></div>
          <div class="question-tamil" id="questionTamil"></div>
          <div class="options" id="optionsContainer"></div>
          <div class="quiz-feedback" id="quizFeedback"></div>
          <div class="quiz-nav">
            <span class="quiz-score-badge" id="scoreBadge">Score: 0</span>
            <button class="btn-primary" id="nextBtn" style="display:none;">Next Question →</button>
          </div>
          <div class="quiz-progress-bar"><div class="quiz-progress-fill" id="qProgressFill" style="width:0%"></div></div>
        </div>
        <div class="quiz-result" id="quizResult">
          <div class="result-score" id="resultScore">0/5</div>
          <div class="result-label" id="resultLabel"></div>
          <button class="btn-primary" onclick="restartQuiz()">Try Again 🔄</button>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <div class="section-inner">
    <p class="section-label">Get In Touch</p>
    <h2 class="section-title">Contact Us<br>தொடர்பு கொள்ளுங்கள்</h2>
    <p class="section-sub">Have a question, suggestion, or want to contribute Tamil automobile content? We'd love to hear from you.</p>
    <div class="contact-grid">
      <div class="contact-info">
        <h3>AutoMaster Tamil</h3>
        <p>We're dedicated to making automobile education accessible in Tamil. Reach out for study support, content queries, or NVQ guidance.</p>
        <div class="contact-item">
          <div class="contact-ico">📧</div>
          <div class="contact-item-text">
            <strong>Email</strong>
            mhdmuhadh76@gmail.com
          </div>
        </div>
        <div class="contact-item">
          <div class="contact-ico">📱</div>
          <div class="contact-item-text">
            <strong>WhatsApp</strong>
            <span>+94 754 668 668</span>
          </div>
        </div>
        <div class="contact-item">
          <div class="contact-ico">📍</div>
          <div class="contact-item-text">
            <strong>Location</strong>
            <span>Sri Lanka</span>
          </div>
        </div>
        <div class="contact-item">
          <div class="contact-ico">🕐</div>
          <div class="contact-item-text">
            <strong>Response Time</strong>
            <span>Within 24 hours</span>
          </div>
        </div>
      </div>
      <form class="contact-form" id="contactForm" onsubmit="submitForm(event)">
        <div class="form-row">
          <div class="form-field">
            <label for="fname">First Name / முதல் பெயர்</label>
            <input type="text" id="fname" placeholder="Mohammad" required />
          </div>
          <div class="form-field">
            <label for="lname">Last Name / கடைசி பெயர்</label>
            <input type="text" id="lname" placeholder="Muhadh" required />
          </div>
        </div>
        <div class="form-field">
          <label for="email">Email</label>
          <input type="email" id="email" placeholder="your@email.com" required />
        </div>
        <div class="form-field">
          <label for="subject">Subject / தலைப்பு</label>
          <select id="subject">
            <option>NVQ Level 3 Enquiry</option>
            <option>Engine Notes Query</option>
            <option>MCQ Feedback</option>
            <option>Content Contribution</option>
            <option>General Question</option>
          </select>
        </div>
        <div class="form-field">
          <label for="message">Message / செய்தி</label>
          <textarea id="message" placeholder="Type your message here…" required></textarea>
        </div>
        <button type="submit" class="btn-primary">Send Message 📨</button>
        <div class="form-success" id="formSuccess">
          ✅ Thank you! Your message has been sent. We'll reply within 24 hours.<br>
          <span style="font-family:var(--font-tamil);font-size:.85rem;">நன்றி! உங்கள் செய்தி அனுப்பப்பட்டது.</span>
        </div>
      </form>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-logo">Auto<span>Master</span> Tamil</div>
  <div class="footer-links">
    <a href="#home">Home</a>
    <a href="#learning">Learning</a>
    <a href="#engine">Engine Notes</a>
    <a href="#nvq">NVQ Level 3</a>
    <a href="#quiz">MCQ Quiz</a>
    <a href="#contact">Contact</a>
  </div>
  <p>© 2025 AutoMaster Tamil. Built for Sri Lanka's Tamil automobile students.</p>
  <p style="margin-top:.4rem;font-family:var(--font-tamil);font-size:.78rem;">தமிழில் ஆட்டோமொபைல் கல்வி — அனைவருக்கும் இலவசம்</p>
</footer>

<button id="scrollTop" onclick="window.scrollTo({top:0,behavior:'smooth'})" aria-label="Scroll to top">↑</button>

<script>
// ── DATA ──────────────────────────────────────────────────────
const learningModules = [
  { icon:'🔧', title:'Engine Fundamentals', tamil:'என்ஜின் அடிப்படைகள்', desc:'4-stroke cycle, combustion principles, engine types (DOHC, SOHC, OHV) and displacement calculations.' },
  { icon:'⚡', title:'Electrical Systems', tamil:'மின் அமைப்புகள்', desc:'Battery, alternator, starter motor, wiring diagrams and circuit diagnosis using a multimeter.' },
  { icon:'🛞', title:'Transmission & Drivetrain', tamil:'டிரான்ஸ்மிஷன் அமைப்பு', desc:'Manual & automatic gearboxes, clutch operation, differential, driveshaft and CV joints.' },
  { icon:'🛑', title:'Braking Systems', tamil:'பிரேக் அமைப்புகள்', desc:'Disc & drum brakes, ABS, brake fluid hydraulics, master cylinder and caliper servicing.' },
  { icon:'🌡️', title:'Cooling System', tamil:'குளிரூட்டல் அமைப்பு', desc:'Coolant flow, radiator, thermostat, water pump, coolant flush procedures and overheating diagnosis.' },
  { icon:'⛽', title:'Fuel & Injection', tamil:'எரிபொருள் & இன்ஜெக்ஷன்', desc:'Fuel pump, injectors, carburettors vs EFI, lambda sensors and mixture control.' },
  { icon:'💨', title:'Exhaust & Emissions', tamil:'வெளியேற்றம் & உமிழ்வுகள்', desc:'Catalytic converter, EGR valve, DPF, lambda testing and emission standards for Sri Lanka.' },
  { icon:'🔩', title:'Suspension & Steering', tamil:'சஸ்பென்ஷன் & ஸ்டீயரிங்', desc:'MacPherson strut, wishbone, rack & pinion, wheel alignment and tyre wear diagnosis.' },
  { icon:'📊', title:'Diagnostics & OBD', tamil:'கண்டறிதல் & OBD', desc:'Reading fault codes, live data, freeze frame, OBD-II protocols and scan tool usage.' },
];

const engineNotes = [
  {
    title:'Four-Stroke Engine Cycle',
    tamil:'நான்கு-ஸ்ட்ரோக் என்ஜின் சுழற்சி',
    content:'The four-stroke cycle is the heart of all modern petrol and diesel engines. Each cycle consists of intake, compression, power and exhaust strokes.',
    points:[
      'Intake Stroke – Piston moves down, inlet valve opens, air-fuel mixture enters.',
      'Compression Stroke – Both valves closed, piston moves up, mixture compressed to 8:1–12:1 ratio.',
      'Power Stroke – Spark ignites mixture, gases expand, piston pushed down (work output).',
      'Exhaust Stroke – Exhaust valve opens, piston moves up, burnt gases expelled.',
    ],
    tag:'Engine Fundamentals'
  },
  {
    title:'Cooling System Operation',
    tamil:'குளிரூட்டல் அமைப்பு செயல்பாடு',
    content:'The cooling system maintains engine temperature between 85°C–95°C using liquid coolant circulated by the water pump.',
    points:[
      'Coolant flows from the water pump through the engine block and cylinder head.',
      'Thermostat remains closed until coolant reaches ~88°C, then opens to allow radiator cooling.',
      'The radiator dissipates heat via airflow — assisted by the cooling fan (electric or belt-driven).',
      'Coolant mixture: 50% antifreeze + 50% distilled water for optimal freeze and boil-over protection.',
    ],
    tag:'Cooling System'
  },
  {
    title:'Fuel Injection Systems (EFI)',
    tamil:'EFI எரிபொருள் உட்செலுத்தல் அமைப்பு',
    content:'Electronic Fuel Injection (EFI) precisely controls fuel delivery using the ECU, sensors, and solenoid injectors for optimum combustion.',
    points:[
      'MAF/MAP sensors measure air intake for fuel calculation.',
      'Oxygen (lambda) sensor provides closed-loop feedback to the ECU.',
      'Fuel pressure: typically 300–400 kPa for port injection systems.',
      'Injector pulse width controlled in milliseconds for precise air-fuel ratio.',
    ],
    tag:'Fuel System'
  },
  {
    title:'Automotive Electrical: Ohm\'s Law',
    tamil:'ஓம் விதி மற்றும் மின்சார அடிப்படைகள்',
    content:"Ohm's Law governs all automotive electrical circuits: Voltage (V) = Current (I) × Resistance (R). Understanding this is essential for fault diagnosis.",
    points:[
      'V = I × R — Voltage equals Current times Resistance.',
      'A 12V battery with a 2Ω load draws 6 amps (I = V/R).',
      'Use a multimeter in voltage, resistance, and continuity modes.',
      'High resistance in a circuit (corroded terminals) causes voltage drop and reduced current.',
    ],
    tag:'Electrical'
  },
  {
    title:'Braking System: Disc Brakes',
    tamil:'டிஸ்க் பிரேக் அமைப்பு',
    content:'Disc brakes use hydraulic pressure to push brake pads against a rotating disc (rotor) to create friction and slow the vehicle.',
    points:[
      'Brake pedal force is amplified by the vacuum servo (brake booster).',
      'Master cylinder converts mechanical force into hydraulic pressure.',
      'Caliper pistons are pushed outward, clamping pads onto the rotor.',
      'Minimum disc thickness must be checked against OEM spec; worn discs must be replaced.',
    ],
    tag:'Braking System'
  },
  {
    title:'OBD-II Fault Codes (DTCs)',
    tamil:'OBD-II தவறு குறியீடுகள்',
    content:'On-Board Diagnostics II (OBD-II) is a standardized system that monitors emissions-related and powertrain components, storing Diagnostic Trouble Codes (DTCs) when faults occur.',
    points:[
      'P-codes: Powertrain | B-codes: Body | C-codes: Chassis | U-codes: Network.',
      'P0300 = Random misfire; P0171 = System lean bank 1; P0420 = Catalyst below threshold.',
      'Freeze frame data captures engine parameters at the moment the fault triggered.',
      'Always verify DTCs with live data before replacing parts.',
    ],
    tag:'Diagnostics'
  },
];

const nvqUnits = [
  {
    code:'LVT 3101', title:'Engine Mechanical Systems', tamil:'என்ஜின் இயந்திர அமைப்புகள்',
    desc:'Diagnose and repair engine mechanical components including cylinder head, pistons, crankshaft and valve train.',
    topics:['Cylinder head overhaul','Timing belt/chain','Valve clearance','Compression test'],
    progress: 85
  },
  {
    code:'LVT 3102', title:'Vehicle Electrical Systems', tamil:'வாகன மின் அமைப்புகள்',
    desc:'Service and repair starting, charging and lighting systems. Read and interpret wiring diagrams.',
    topics:['Battery testing','Alternator output','Starter circuit','Wiring diagrams'],
    progress: 70
  },
  {
    code:'LVT 3103', title:'Fuel & Emission Control', tamil:'எரிபொருள் & வெளியேற்ற கட்டுப்பாடு',
    desc:'Diagnose fuel delivery and emission control systems, including EFI, catalytic converters and EGR.',
    topics:['EFI diagnosis','Lambda sensors','Catalytic converter','Emission testing'],
    progress: 60
  },
  {
    code:'LVT 3104', title:'Transmission Systems', tamil:'டிரான்ஸ்மிஷன் அமைப்புகள்',
    desc:'Service manual and automatic transmissions, clutch assemblies and drive line components.',
    topics:['Clutch adjustment','Gearbox oil change','CV joint replacement','Differential service'],
    progress: 75
  },
  {
    code:'LVT 3105', title:'Brake & Suspension Systems', tamil:'பிரேக் & சஸ்பென்ஷன்',
    desc:'Inspect, diagnose and repair hydraulic braking, ABS and suspension and steering systems.',
    topics:['Brake pad replacement','ABS diagnosis','Wheel alignment','Shock absorber testing'],
    progress: 80
  },
  {
    code:'LVT 3106', title:'Vehicle Air Conditioning', tamil:'வாகன ஏர் கண்டிஷனர்',
    desc:'Service refrigerant systems, diagnose compressor, condenser, evaporator and control systems.',
    topics:['Refrigerant recovery','Compressor clutch','Evaporator service','AC diagnosis'],
    progress: 50
  },
];

const quizCategories = {
  Engine: [
    { q:'What is the compression ratio range for a typical petrol engine?', qt:'பெட்ரோல் என்ஜினில் இயக்க விகிதம் என்ன?', opts:['4:1 to 6:1','8:1 to 12:1','15:1 to 22:1','1:1 to 3:1'], ans:1, exp:'Petrol engines typically compress the air-fuel mixture at a ratio of 8:1 to 12:1 before ignition.' },
    { q:'Which stroke produces the power output in a 4-stroke engine?', qt:'4-ஸ்ட்ரோக் என்ஜினில் எந்த ஸ்ட்ரோக் சக்தியை உருவாக்குகிறது?', opts:['Intake','Compression','Power','Exhaust'], ans:2, exp:'The power (combustion) stroke is the only stroke that produces work. The burning gases expand and push the piston down.' },
    { q:'What does TDC stand for in engine terminology?', qt:'என்ஜின் சொல்லாட்சியில் TDC என்றால் என்ன?', opts:['Top Dead Centre','Total Drive Combustion','Torque Delivery Control','Timing Diesel Calibration'], ans:0, exp:'TDC = Top Dead Centre — the position of the piston at its highest point in the cylinder.' },
    { q:'Which sensor measures incoming air mass in a modern EFI system?', qt:'EFI அமைப்பில் உட்வரும் காற்று நிறை அளவிடும் சென்சார் எது?', opts:['O2 Sensor','TPS','MAF Sensor','MAP Sensor'], ans:2, exp:'The MAF (Mass Airflow) sensor directly measures the mass of air entering the engine to calculate correct fuel injection.' },
    { q:'What is the purpose of the thermostat in the cooling system?', qt:'குளிரூட்டல் அமைப்பில் தெர்மோஸ்டேட்டின் நோக்கம் என்ன?', opts:['Control fuel flow','Regulate coolant temperature','Monitor oil pressure','Detect exhaust leaks'], ans:1, exp:'The thermostat regulates coolant temperature by controlling when coolant flows to the radiator, maintaining optimal engine temperature.' },
  ],
  Electrical: [
    { q:'What is the standard voltage of a fully charged automotive battery?', qt:'கார் பேட்டரியின் நிரல் மின்னழுத்தம் எவ்வளவு?', opts:['6V','10.5V','12.6V','15V'], ans:2, exp:'A fully charged 12V lead-acid battery reads approximately 12.6V at rest (open circuit voltage).' },
    { q:'Which law states V = I × R?', qt:'V = I × R என்பது எந்த விதி?', opts:["Newton's Law","Ohm's Law","Faraday's Law","Kirchhoff's Law"], ans:1, exp:"Ohm's Law: Voltage = Current × Resistance. This fundamental law applies to all automotive electrical circuits." },
    { q:'The alternator in a vehicle is driven by which component?', qt:'மாற்றி (alternator) எந்த பாகத்தால் இயக்கப்படுகிறது?', opts:['Camshaft','Timing chain','Serpentine belt','Flywheel'], ans:2, exp:'The alternator is belt-driven from the crankshaft pulley via the serpentine (or accessory) belt.' },
    { q:'What does a CAN Bus system do in modern vehicles?', qt:'நவீன வாகனங்களில் CAN Bus அமைப்பு என்ன செய்கிறது?', opts:['Controls air conditioning only','Allows ECUs to communicate','Measures fuel pressure','Controls the throttle only'], ans:1, exp:'CAN (Controller Area Network) Bus allows multiple Electronic Control Units (ECUs) to communicate with each other over a shared serial bus.' },
    { q:'Which tool is used to measure electrical resistance in a circuit?', qt:'மின்சார எதிர்ப்பை அளவிட எந்த கருவி பயன்படுகிறது?', opts:['Pressure gauge','Oscilloscope','Multimeter','Vacuum gauge'], ans:2, exp:'A multimeter (set to ohm mode, Ω) is used to measure resistance in automotive circuits.' },
  ],
  NVQ: [
    { q:'What must be checked before replacing a brake disc on a light vehicle?', qt:'பிரேக் டிஸ்கை மாற்றும் முன் என்ன சரிபார்க்க வேண்டும்?', opts:['Engine oil level','Minimum disc thickness specification','Air filter condition','Tyre pressure'], ans:1, exp:'Always check OEM minimum disc thickness specification. If the disc is worn beyond minimum, it must be replaced.' },
    { q:'What is the purpose of wheel alignment?', qt:'சக்கர சீரமைப்பின் நோக்கம் என்ன?', opts:['Increase fuel consumption','Ensure tyres wear evenly and vehicle tracks straight','Reduce engine power','Change gear ratios'], ans:1, exp:'Correct wheel alignment ensures even tyre wear, proper vehicle handling and straight-line stability.' },
    { q:'Which NVQ Level 3 unit covers EFI diagnosis?', qt:'EFI கண்டறிதலை உள்ளடக்கிய NVQ நிலை 3 அலகு எது?', opts:['LVT 3101','LVT 3102','LVT 3103','LVT 3104'], ans:2, exp:'LVT 3103 – Fuel & Emission Control covers EFI system diagnosis, lambda sensors and catalytic converter testing.' },
    { q:'What is the correct clutch pedal free play for most light vehicles?', qt:'கிளட்ச் பெடல் இலவச விளையாட்டு என்ன?', opts:['0 mm (no free play)','5–15 mm','50–100 mm','200 mm'], ans:1, exp:'Typical clutch pedal free play is 5–15 mm. Zero free play causes clutch slip; excessive free play causes incomplete disengagement.' },
    { q:'When using an OBD-II scanner, P0300 indicates what fault?', qt:'P0300 குறியீடு என்ன தவறை குறிக்கிறது?', opts:['Fuel pressure low','Random/multiple cylinder misfires','O2 sensor fault','Transmission slip'], ans:1, exp:'DTC P0300 = Random or Multiple Cylinder Misfire Detected. It means the engine is misfiring but not isolated to one cylinder.' },
  ]
};

// ── RENDER LEARNING CARDS ───────────────────────────────────
function renderLearning() {
  const grid = document.getElementById('learnGrid');
  grid.innerHTML = learningModules.map(m => `
    <div class="learn-card" tabindex="0">
      <div class="learn-icon">${m.icon}</div>
      <h3>${m.title}</h3>
      <p class="tamil-sub">${m.tamil}</p>
      <p>${m.desc}</p>
    </div>
  `).join('');
}

// ── RENDER ACCORDION ────────────────────────────────────────
function renderAccordion() {
  const acc = document.getElementById('accordion');
  acc.innerHTML = engineNotes.map((n, i) => `
    <div class="acc-item" id="acc${i}">
      <button class="acc-head" onclick="toggleAcc(${i})" aria-expanded="false">
        <span>${n.title} <small style="font-family:var(--font-tamil);font-weight:400;font-size:.8rem;color:var(--muted);"> — ${n.tamil}</small></span>
        <span class="acc-arrow">▾</span>
      </button>
      <div class="acc-body">
        <p>${n.content}</p>
        <ul>${n.points.map(p=>`<li>${p}</li>`).join('')}</ul>
        <span class="note-tag">${n.tag}</span>
      </div>
    </div>
  `).join('');
}

function toggleAcc(i) {
  const item = document.getElementById('acc'+i);
  const isOpen = item.classList.contains('open');
  document.querySelectorAll('.acc-item.open').forEach(el => el.classList.remove('open'));
  if (!isOpen) item.classList.add('open');
}

// ── RENDER NVQ CARDS ────────────────────────────────────────
function renderNVQ() {
  const grid = document.getElementById('nvqGrid');
  grid.innerHTML = nvqUnits.map(u => `
    <div class="nvq-card">
      <div class="nvq-card-head">
        <div class="unit-code">${u.code}</div>
        <h3>${u.title}</h3>
        <div class="tamil">${u.tamil}</div>
      </div>
      <div class="nvq-card-body">
        <p>${u.desc}</p>
        <div class="nvq-topics">${u.topics.map(t=>`<span>${t}</span>`).join('')}</div>
        <div class="nvq-progress">
          <div class="progress-label"><span>Study Progress</span><span>${u.progress}%</span></div>
          <div class="progress-bar"><div class="progress-fill" style="width:${u.progress}%"></div></div>
        </div>
      </div>
    </div>
  `).join('');
}

// ── QUIZ ENGINE ─────────────────────────────────────────────
let currentCat = 'Engine';
let currentQ = 0;
let score = 0;
let answered = false;

function renderCatTabs() {
  const tabs = document.getElementById('catTabs');
  tabs.innerHTML = Object.keys(quizCategories).map(cat => `
    <button class="quiz-tab ${cat===currentCat?'active':''}" onclick="switchCat('${cat}')">${cat}</button>
  `).join('');
}

function switchCat(cat) {
  currentCat = cat;
  currentQ = 0; score = 0; answered = false;
  document.getElementById('quizResult').classList.remove('show');
  document.getElementById('quizQuestion').style.display = '';
  document.getElementById('quizCatLabel').textContent = cat;
  renderCatTabs();
  renderQuestion();
}

function renderQuestion() {
  const questions = quizCategories[currentCat];
  const q = questions[currentQ];
  const total = questions.length;

  document.getElementById('questionNum').textContent = `Question ${currentQ+1} of ${total}`;
  document.getElementById('qNum').textContent = currentQ+1;
  document.getElementById('qTotal').textContent = total;
  document.getElementById('questionText').textContent = q.q;
  document.getElementById('questionTamil').textContent = q.qt;
  document.getElementById('quizFeedback').className = 'quiz-feedback';
  document.getElementById('quizFeedback').textContent = '';
  document.getElementById('nextBtn').style.display = 'none';
  document.getElementById('qProgressFill').style.width = `${(currentQ/total)*100}%`;

  const letters = ['A','B','C','D'];
  const opts = document.getElementById('optionsContainer');
  opts.innerHTML = q.opts.map((o,i) => `
    <button class="opt-btn" onclick="selectOpt(${i})" id="opt${i}">
      <span class="opt-letter">${letters[i]}</span> ${o}
    </button>
  `).join('');
  answered = false;
}

function selectOpt(i) {
  if (answered) return;
  answered = true;
  const q = quizCategories[currentCat][currentQ];
  const fb = document.getElementById('quizFeedback');

  document.querySelectorAll('.opt-btn').forEach(btn => btn.disabled = true);

  const selectedBtn = document.getElementById('opt'+i);
  const correctBtn = document.getElementById('opt'+q.ans);

  if (i === q.ans) {
    selectedBtn.classList.add('correct');
    score++;
    fb.className = 'quiz-feedback correct-fb show';
    fb.textContent = '✅ Correct! ' + q.exp;
  } else {
    selectedBtn.classList.add('wrong');
    correctBtn.classList.add('correct');
    fb.className = 'quiz-feedback wrong-fb show';
    fb.textContent = '❌ Incorrect. ' + q.exp;
  }

  updateScore();
  document.getElementById('nextBtn').style.display = 'inline-block';
}

function updateScore() {
  document.getElementById('scoreBadge').textContent = `Score: ${score}`;
  document.getElementById('scoreLive').textContent = score;
}

document.getElementById('nextBtn')?.addEventListener('click', () => {
  const total = quizCategories[currentCat].length;
  currentQ++;
  if (currentQ >= total) {
    showResult();
  } else {
    renderQuestion();
  }
});

function showResult() {
  document.getElementById('quizQuestion').style.display = 'none';
  const res = document.getElementById('quizResult');
  const total = quizCategories[currentCat].length;
  res.classList.add('show');
  document.getElementById('resultScore').textContent = `${score}/${total}`;
  const pct = (score/total)*100;
  let label = pct === 100 ? '🏆 Perfect Score! Excellent work!' :
              pct >= 80  ? '🎉 Great job! Almost there.' :
              pct >= 60  ? '👍 Good effort. Keep studying.' :
                           '📚 Keep practising — you can do it!';
  document.getElementById('resultLabel').textContent = label;
}

function restartQuiz() {
  currentQ = 0; score = 0; answered = false;
  document.getElementById('quizResult').classList.remove('show');
  document.getElementById('quizQuestion').style.display = '';
  updateScore();
  renderQuestion();
}

// ── FORM ────────────────────────────────────────────────────
function submitForm(e) {
  e.preventDefault();
  document.getElementById('contactForm').style.display = 'none';
  document.getElementById('formSuccess').classList.add('show');
}

// ── DARK MODE ────────────────────────────────────────────────
const themeBtn = document.getElementById('themeToggle');
let isDark = true;
themeBtn.addEventListener('click', () => {
  isDark = !isDark;
  document.documentElement.setAttribute('data-theme', isDark ? '' : 'light');
  themeBtn.textContent = isDark ? '🌙' : '☀️';
});

// ── HAMBURGER ────────────────────────────────────────────────
document.getElementById('hamburger').addEventListener('click', function() {
  const menu = document.getElementById('mobileMenu');
  const open = menu.classList.toggle('open');
  this.setAttribute('aria-expanded', open);
});
document.querySelectorAll('.mobile-menu a').forEach(a => {
  a.addEventListener('click', () => {
    document.getElementById('mobileMenu').classList.remove('open');
  });
});

// ── ACTIVE NAV LINK ──────────────────────────────────────────
const sections = document.querySelectorAll('section[id]');
const navLinks = document.querySelectorAll('.nav-links a');
window.addEventListener('scroll', () => {
  let current = '';
  sections.forEach(sec => {
    if (window.scrollY >= sec.offsetTop - 100) current = sec.id;
  });
  navLinks.forEach(a => {
    a.classList.toggle('active', a.getAttribute('href') === '#'+current);
  });
  // scroll to top
  const btn = document.getElementById('scrollTop');
  btn.classList.toggle('visible', window.scrollY > 300);
}, { passive:true });

// ── INIT ─────────────────────────────────────────────────────
renderLearning();
renderAccordion();
renderNVQ();
renderCatTabs();
renderQuestion();
</script>
</body>
</html>
