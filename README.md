<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>anita zaharaa — GitHub README</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Mono:wght@400;500&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet"/>
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    background: #f0ebe4;
    display: flex;
    justify-content: center;
    align-items: flex-start;
    min-height: 100vh;
    padding: 2rem 1rem;
    font-family: 'DM Sans', sans-serif;
  }

  .readme-wrap {
    width: 100%;
    max-width: 680px;
    background: #f5f0eb;
    border-radius: 16px;
    overflow: hidden;
    border: 0.5px solid #ddd5c8;
    color: #3a322c;
  }

  .readme-header {
    background: linear-gradient(135deg, #e8ddd4 0%, #d4c5b8 50%, #c2b0a2 100%);
    padding: 2.5rem 2rem 2rem;
    text-align: center;
    position: relative;
    border-bottom: 0.5px solid #c9b8aa;
  }

  .readme-header::before {
    content: '';
    position: absolute;
    inset: 0;
    background: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23b8a090' fill-opacity='0.15'%3E%3Ccircle cx='30' cy='30' r='1'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
    opacity: 0.6;
  }

  .readme-name {
    font-family: 'DM Serif Display', serif;
    font-size: 2.8rem;
    color: #3a2f27;
    margin: 0 0 0.25rem;
    position: relative;
    letter-spacing: -0.5px;
  }

  .readme-tagline {
    font-size: 0.8rem;
    color: #7a6558;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    position: relative;
    margin: 0 0 1.25rem;
  }

  .typing-row {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    justify-content: center;
    position: relative;
  }

  .typing-pill {
    background: rgba(255,255,255,0.55);
    border: 0.5px solid rgba(255,255,255,0.8);
    border-radius: 999px;
    padding: 5px 14px;
    font-size: 0.75rem;
    color: #5a4a3e;
    font-weight: 500;
  }

  .readme-body {
    padding: 1.75rem;
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
  }

  .code-block {
    background: #ede7e0;
    border: 0.5px solid #d4c5b8;
    border-radius: 10px;
    padding: 1.1rem 1.25rem;
    font-family: 'DM Mono', monospace;
    font-size: 0.78rem;
    color: #5a4438;
    line-height: 1.75;
  }

  .code-kw  { color: #a06040; font-weight: 500; }
  .code-str { color: #6b8a60; }
  .code-var { color: #7060a0; }
  .code-key { color: #5a4438; }

  .section-label {
    font-size: 0.68rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: #9e8878;
    margin-bottom: 0.75rem;
    font-weight: 500;
  }

  .stats-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;
  }

  .stat-card {
    background: #ede7e0;
    border: 0.5px solid #d4c5b8;
    border-radius: 10px;
    padding: 1rem 1.1rem;
  }

  .stat-card-label {
    font-size: 0.7rem;
    color: #9e8878;
    margin-bottom: 0.35rem;
    text-transform: uppercase;
    letter-spacing: 0.1em;
  }

  .stat-card-val {
    font-size: 1.5rem;
    font-weight: 500;
    color: #3a2f27;
    font-family: 'DM Serif Display', serif;
  }

  .stat-card-sub {
    font-size: 0.72rem;
    color: #7a6558;
    margin-top: 2px;
  }

  .skills-row {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  .skill-tag {
    background: #ede7e0;
    border: 0.5px solid #c9b8aa;
    border-radius: 999px;
    padding: 5px 14px;
    font-size: 0.75rem;
    color: #5a4438;
    font-weight: 500;
    display: flex;
    align-items: center;
    gap: 6px;
  }

  .skill-dot {
    width: 6px;
    height: 6px;
    border-radius: 50%;
    flex-shrink: 0;
  }

  .streak-bar-wrap {
    background: #ede7e0;
    border: 0.5px solid #d4c5b8;
    border-radius: 10px;
    padding: 1rem 1.25rem;
  }

  .streak-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 0.75rem;
  }

  .streak-title { font-size: 0.78rem; color: #7a6558; }

  .streak-num {
    font-family: 'DM Serif Display', serif;
    font-size: 1.6rem;
    color: #3a2f27;
  }

  .bar-track {
    background: #d4c5b8;
    border-radius: 999px;
    height: 6px;
    margin-bottom: 6px;
    overflow: hidden;
  }

  .bar-fill {
    height: 100%;
    border-radius: 999px;
  }

  .bar-label {
    display: flex;
    justify-content: space-between;
    font-size: 0.68rem;
    color: #9e8878;
  }

  .lang-row { margin-bottom: 10px; }

  .quote-block {
    background: #ede7e0;
    border-left: 3px solid #b8a090;
    border-radius: 0 10px 10px 0;
    padding: 1rem 1.25rem;
    font-family: 'DM Serif Display', serif;
    font-style: italic;
    font-size: 0.9rem;
    color: #5a4438;
    line-height: 1.6;
  }

  .quote-attr {
    font-family: 'DM Sans', sans-serif;
    font-style: normal;
    font-size: 0.7rem;
    color: #9e8878;
    margin-top: 6px;
    letter-spacing: 0.08em;
    text-transform: uppercase;
  }

  .views-footer {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
    padding: 1rem;
    border-top: 0.5px solid #d4c5b8;
    font-size: 0.72rem;
    color: #9e8878;
  }

  .views-badge {
    background: #d4c5b8;
    border-radius: 999px;
    padding: 3px 12px;
    color: #5a4438;
    font-weight: 500;
  }

  .readme-footer-wave {
    height: 40px;
    background: linear-gradient(135deg, #c2b0a2 0%, #d4c5b8 50%, #e8ddd4 100%);
  }
</style>
</head>
<body>
<div class="readme-wrap">

  <!-- HEADER -->
  <div class="readme-header">
    <div class="readme-name">Anita Zahara</div>
    <div class="readme-tagline">frontend developer · vue lover · pixel perfectionist</div>
    <div class="typing-row">
      <span class="typing-pill">Hello there! 🌸</span>
      <span class="typing-pill">Vue.js &amp; TypeScript</span>
      <span class="typing-pill">One commit a day keeps bugs away 🐛</span>
    </div>
  </div>

  <!-- BODY -->
  <div class="readme-body">

    <!-- About -->
    <div>
      <div class="section-label">about me</div>
      <div class="code-block">
        <span class="code-kw">const</span> <span class="code-var">anita</span> = {<br>
        &nbsp;&nbsp;<span class="code-key">name</span>: <span class="code-str">"Anita Zaharaa"</span>,<br>
        &nbsp;&nbsp;<span class="code-key">role</span>: <span class="code-str">"Frontend Developer"</span>,<br>
        &nbsp;&nbsp;<span class="code-key">loves</span>: [<span class="code-str">"Vue.js"</span>, <span class="code-str">"TypeScript"</span>, <span class="code-str">"clean UI"</span>, <span class="code-str">"iced coffee ☕"</span>],<br>
        &nbsp;&nbsp;<span class="code-key">currently</span>: <span class="code-str">"building things that look good &amp; work well"</span>,<br>
        };
      </div>
    </div>

    <!-- Stack -->
    <div>
      <div class="section-label">stack</div>
      <div class="skills-row">
        <span class="skill-tag"><span class="skill-dot" style="background:#42b883"></span>Vue.js</span>
        <span class="skill-tag"><span class="skill-dot" style="background:#3178c6"></span>TypeScript</span>
        <span class="skill-tag"><span class="skill-dot" style="background:#007acc"></span>VS Code</span>
        <span class="skill-tag"><span class="skill-dot" style="background:#333"></span>GitHub</span>
        <span class="skill-tag"><span class="skill-dot" style="background:#fc6d26"></span>GitLab</span>
        <span class="skill-tag"><span class="skill-dot" style="background:#4285f4"></span>Chrome DevTools</span>
      </div>
    </div>

    <!-- GitHub Stats -->
    <div>
      <div class="section-label">github stats</div>
      <div class="stats-grid">
        <div class="stat-card">
          <div class="stat-card-label">total commits</div>
          <div class="stat-card-val">847</div>
          <div class="stat-card-sub">across all repos</div>
        </div>
        <div class="stat-card">
          <div class="stat-card-label">top language</div>
          <div class="stat-card-val">Vue</div>
          <div class="stat-card-sub">68% of codebase</div>
        </div>
        <div class="stat-card">
          <div class="stat-card-label">pull requests</div>
          <div class="stat-card-val">124</div>
          <div class="stat-card-sub">merged</div>
        </div>
        <div class="stat-card">
          <div class="stat-card-label">stars earned</div>
          <div class="stat-card-val">312</div>
          <div class="stat-card-sub">across projects</div>
        </div>
      </div>
    </div>

    <!-- Language Breakdown -->
    <div>
      <div class="section-label">language breakdown</div>
      <div class="streak-bar-wrap">
        <div class="lang-row">
          <div class="bar-label" style="margin-bottom:4px"><span>Vue.js</span><span>68%</span></div>
          <div class="bar-track"><div class="bar-fill" style="width:68%;background:#42b883"></div></div>
        </div>
        <div class="lang-row">
          <div class="bar-label" style="margin-bottom:4px"><span>TypeScript</span><span>20%</span></div>
          <div class="bar-track"><div class="bar-fill" style="width:20%;background:#3178c6"></div></div>
        </div>
        <div class="lang-row">
          <div class="bar-label" style="margin-bottom:4px"><span>CSS</span><span>9%</span></div>
          <div class="bar-track"><div class="bar-fill" style="width:9%;background:#c9b8aa"></div></div>
        </div>
        <div class="lang-row">
          <div class="bar-label" style="margin-bottom:4px"><span>Other</span><span>3%</span></div>
          <div class="bar-track"><div class="bar-fill" style="width:3%;background:#b8a090"></div></div>
        </div>
      </div>
    </div>

    <!-- Streak -->
    <div>
      <div class="section-label">current streak</div>
      <div class="streak-bar-wrap">
        <div class="streak-row">
          <span class="streak-title">days in a row</span>
          <span class="streak-num">21 🔥</span>
        </div>
        <div class="bar-track">
          <div class="bar-fill" style="width:70%;background:linear-gradient(90deg,#c2b0a2,#a09080)"></div>
        </div>
        <div class="bar-label"><span>started May 13</span><span>best: 34 days</span></div>
      </div>
    </div>

    <!-- Quote -->
    <div>
      <div class="section-label">quote of the day</div>
      <div class="quote-block">
        "Any fool can write code that a computer can understand. Good programmers write code that humans can understand."
        <div class="quote-attr">— Martin Fowler</div>
      </div>
    </div>

  </div>

  <!-- FOOTER -->
  <div class="views-footer">
    <span>profile views</span>
    <span class="views-badge">anitazaharaa</span>
    <span>· thanks for stopping by 🌿</span>
  </div>
  <div class="readme-footer-wave"></div>

</div>
</body>
</html>
