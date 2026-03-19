<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>s8n0gre — GitHub Profile</title>
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;600;700&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet" />
<style>
  :root {
    --bg: #0d1117;
    --surface: #161b22;
    --border: #21262d;
    --green: #00ff41;
    --blue: #58a6ff;
    --muted: #9fb3c8;
    --text: #c9d1d9;
    --accent2: #238636;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: 'JetBrains Mono', monospace;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    padding: 40px 16px 60px;
  }

  .page {
    width: 100%;
    max-width: 760px;
    display: flex;
    flex-direction: column;
    gap: 0;
  }

  /* ── HEADER ── */
  .header {
    background: linear-gradient(135deg, #000 60%, #001a00);
    border: 1px solid #1a3a1a;
    border-radius: 12px 12px 0 0;
    padding: 36px 24px 28px;
    text-align: center;
    position: relative;
    overflow: hidden;
  }
  .header::before {
    content: '';
    position: absolute;
    inset: 0;
    background: radial-gradient(ellipse at 50% 0%, rgba(0,255,65,0.07) 0%, transparent 70%);
    pointer-events: none;
  }
  .header .blink {
    display: inline-block;
    color: var(--green);
    font-size: 13px;
    letter-spacing: 2px;
    font-weight: 600;
    margin-bottom: 10px;
    opacity: 0.8;
  }
  .header h1 {
    font-family: 'Space Mono', monospace;
    font-size: clamp(28px, 6vw, 46px);
    font-weight: 700;
    color: var(--green);
    letter-spacing: 4px;
    text-shadow: 0 0 24px rgba(0,255,65,0.4);
    margin-bottom: 6px;
  }
  .header .sub {
    color: var(--muted);
    font-size: 14px;
    letter-spacing: 1px;
    margin-bottom: 18px;
  }
  .typing-row {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 8px;
  }
  .typing-row span {
    background: rgba(88,166,255,0.08);
    border: 1px solid rgba(88,166,255,0.2);
    color: var(--blue);
    font-size: 12px;
    padding: 4px 12px;
    border-radius: 20px;
    letter-spacing: 0.5px;
  }

  /* ── SECTION WRAPPER ── */
  .section {
    border-left: 1px solid var(--border);
    border-right: 1px solid var(--border);
    padding: 32px 28px;
    background: var(--surface);
  }
  .section + .section {
    border-top: 1px solid var(--border);
  }
  .section:last-child {
    border-radius: 0 0 12px 12px;
    border-bottom: 1px solid var(--border);
  }

  .section-label {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 22px;
  }
  .section-label h2 {
    font-size: 13px;
    font-weight: 700;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--blue);
  }
  .section-label::after {
    content: '';
    flex: 1;
    height: 1px;
    background: linear-gradient(to right, var(--border), transparent);
  }

  /* ── TECH STACK ── */
  .tech-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
    gap: 10px;
  }
  .tech-badge {
    display: flex;
    align-items: center;
    gap: 10px;
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 10px 14px;
    font-size: 13px;
    color: var(--text);
    transition: border-color 0.2s, transform 0.2s;
    cursor: default;
  }
  .tech-badge:hover {
    border-color: var(--blue);
    transform: translateY(-2px);
  }
  .tech-badge .dot {
    width: 8px;
    height: 8px;
    border-radius: 50%;
    flex-shrink: 0;
  }

  /* ── METRICS (images) ── */
  .metrics-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 16px;
  }
  .metric-card {
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 6px;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }
  .metric-card img {
    width: 100%;
    height: auto;
    border-radius: 6px;
    display: block;
  }

  /* ── FOCUS BADGES ── */
  .focus-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 12px;
  }
  .focus-card {
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 14px 16px;
    display: flex;
    flex-direction: column;
    gap: 4px;
  }
  .focus-card .label {
    font-size: 10px;
    letter-spacing: 2px;
    color: var(--muted);
    text-transform: uppercase;
  }
  .focus-card .value {
    font-size: 13px;
    color: var(--text);
    font-weight: 600;
  }
  .focus-card.green { border-left: 3px solid var(--accent2); }
  .focus-card.blue  { border-left: 3px solid var(--blue); }
  .focus-card.dim   { border-left: 3px solid #30363d; }

  /* ── YAML BLOCK ── */
  .yaml-block {
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 20px 22px;
    font-size: 13px;
    line-height: 1.9;
    overflow-x: auto;
  }
  .yaml-key   { color: var(--blue); font-weight: 700; }
  .yaml-sub   { color: var(--muted); }
  .yaml-val   { color: #a5d6a7; }
  .yaml-comment { color: #484f58; }
  .yaml-indent1 { padding-left: 20px; }
  .yaml-indent2 { padding-left: 40px; }

  /* ── SNAKE ── */
  .snake-wrap {
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 10px;
    overflow: hidden;
  }
  .snake-wrap img {
    width: 100%;
    height: auto;
    display: block;
    border-radius: 6px;
  }

  /* ── ACTIVITY GRAPH ── */
  .activity-wrap {
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 10px;
    overflow: hidden;
  }
  .activity-wrap img {
    width: 100%;
    height: auto;
    display: block;
    border-radius: 6px;
  }

  /* ── FOOTER ── */
  .footer {
    margin-top: 20px;
    text-align: center;
    font-size: 11px;
    color: #484f58;
    letter-spacing: 1px;
  }

  @media (max-width: 500px) {
    .section { padding: 24px 16px; }
    .tech-grid { grid-template-columns: repeat(2, 1fr); }
  }
</style>
</head>
<body>
<div class="page">

  <!-- HEADER -->
  <div class="header">
    <div class="blink">&gt; ACCESS GRANTED &nbsp;|&nbsp; SYSTEM ONLINE</div>
    <h1>s8n0gre</h1>
    <div class="sub">Software Engineering Student</div>
    <div class="typing-row">
      <span>Data Structures &amp; Algorithms</span>
      <span>Systematic Problem Solving</span>
      <span>Chess-Driven Thinking</span>
    </div>
  </div>

  <!-- CONTRIBUTION SNAKE -->
  <div class="section">
    <div class="section-label"><h2>Contribution Graph</h2></div>
    <div class="snake-wrap">
      <img
        src="https://raw.githubusercontent.com/s8n0gre/s8n0gre/output/github-contribution-grid-snake.svg"
        alt="Contribution snake animation"
      />
    </div>
  </div>

  <!-- TECH STACK -->
  <div class="section">
    <div class="section-label"><h2>Tech Stack</h2></div>
    <div class="tech-grid">
      <div class="tech-badge"><span class="dot" style="background:#004CC7"></span>C++</div>
      <div class="tech-badge"><span class="dot" style="background:#E76F00"></span>Java</div>
      <div class="tech-badge"><span class="dot" style="background:#3776AB"></span>Python</div>
      <div class="tech-badge"><span class="dot" style="background:#FACC15"></span>JavaScript</div>
      <div class="tech-badge"><span class="dot" style="background:#E5533D"></span>HTML</div>
      <div class="tech-badge"><span class="dot" style="background:#1572B6"></span>CSS</div>
      <div class="tech-badge"><span class="dot" style="background:#F05032"></span>Git</div>
      <div class="tech-badge"><span class="dot" style="background:#6e7681"></span>GitHub</div>
    </div>
  </div>

  <!-- GITHUB METRICS -->
  <div class="section">
    <div class="section-label"><h2>GitHub Metrics</h2></div>
    <div class="metrics-grid">
      <div class="metric-card">
        <img
          src="https://github-readme-stats.vercel.app/api?username=s8n0gre&show_icons=true&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=58A6FF&icon_color=58A6FF&text_color=C9D1D9"
          alt="GitHub stats"
        />
      </div>
      <div class="metric-card">
        <img
          src="https://streak-stats.demolab.com?user=s8n0gre&theme=github-dark-blue&hide_border=true&background=0D1117&ring=58A6FF&fire=58A6FF&currStreakLabel=9FB3C8"
          alt="GitHub streak"
        />
      </div>
    </div>
  </div>

  <!-- ACTIVITY GRAPH -->
  <div class="section">
    <div class="section-label"><h2>Activity Overview</h2></div>
    <div class="activity-wrap">
      <img
        src="https://github-readme-activity-graph.vercel.app/graph?username=s8n0gre&theme=github-dark&bg_color=0d1117&color=58A6FF&line=58A6FF&point=C9D1D9&area=true&hide_border=true"
        alt="Activity graph"
      />
    </div>
  </div>

  <!-- FOCUS AREAS -->
  <div class="section">
    <div class="section-label"><h2>Focus Areas</h2></div>
    <div class="focus-grid">
      <div class="focus-card blue">
        <span class="label">Focus</span>
        <span class="value">Data Structures &amp; Algorithms</span>
      </div>
      <div class="focus-card dim">
        <span class="label">Approach</span>
        <span class="value">Analytical Thinking</span>
      </div>
      <div class="focus-card green">
        <span class="label">Status</span>
        <span class="value">Continuous Learning</span>
      </div>
    </div>
  </div>

  <!-- 2026 OBJECTIVES -->
  <div class="section">
    <div class="section-label"><h2>2026 Objectives</h2></div>
    <div class="yaml-block">
      <div><span class="yaml-key">DSA</span><span class="yaml-sub">:</span></div>
      <div class="yaml-indent1"><span class="yaml-sub">target</span><span class="yaml-sub">: </span><span class="yaml-val">300+ problems</span></div>
      <div class="yaml-indent1"><span class="yaml-sub">focus</span><span class="yaml-sub">: </span><span class="yaml-val">arrays, trees, graphs, dynamic programming</span></div>
      <br/>
      <div><span class="yaml-key">Development</span><span class="yaml-sub">:</span></div>
      <div class="yaml-indent1"><span class="yaml-sub">goal</span><span class="yaml-sub">: </span><span class="yaml-val">consistent project building</span></div>
      <div class="yaml-indent1"><span class="yaml-sub">stack</span><span class="yaml-sub">: </span><span class="yaml-val">frontend + backend fundamentals</span></div>
      <br/>
      <div><span class="yaml-key">Growth</span><span class="yaml-sub">:</span></div>
      <div class="yaml-indent1"><span class="yaml-sub">improve</span><span class="yaml-sub">: </span><span class="yaml-val">problem solving speed</span></div>
      <div class="yaml-indent1"><span class="yaml-sub">practice</span><span class="yaml-sub">: </span><span class="yaml-val">daily consistency</span></div>
    </div>
  </div>

  <div class="footer">&gt; s8n0gre &nbsp;·&nbsp; 2026 &nbsp;·&nbsp; ALWAYS LEARNING</div>
</div>
</body>
</html>
