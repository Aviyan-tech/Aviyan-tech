<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Trophy Case</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600&family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@500&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #F7F6F2;
    --card: #FFFFFF;
    --border: #E4E1D8;
    --text: #1C1B18;
    --text-secondary: #6B6960;
    --text-muted: #A6A399;
    --gold-bg: #FBF1DC;
    --gold-text: #8A5A0B;
    --gold-icon: #C6870F;
    --purple-bg: #EFEBFB;
    --purple-text: #5B3FA0;
    --purple-icon: #7C5CD6;
    --blue-bg: #E8F1FB;
    --blue-text: #1D5A96;
    --blue-icon: #3480CC;
    --radius: 14px;
    --font-display: "Space Grotesk", sans-serif;
    --font-body: "Inter", sans-serif;
    --font-mono: "IBM Plex Mono", monospace;
  }

  @media (prefers-color-scheme: dark) {
    :root {
      --bg: #14151A;
      --card: #1D1F26;
      --border: #2C2E37;
      --text: #EDEBE3;
      --text-secondary: #9C9C9C;
      --gold-bg: #33290F;
      --gold-text: #E8B84B;
      --gold-icon: #E8B84B;
      --purple-bg: #251F3A;
      --purple-text: #B9A3F5;
      --purple-icon: #B9A3F5;
      --blue-bg: #16273A;
      --blue-text: #7EB3EA;
      --blue-icon: #7EB3EA;
    }
  }

  * { box-sizing: border-box; }

  body {
    margin: 0;
    padding: 48px 24px;
    background: var(--bg);
    font-family: var(--font-body);
    color: var(--text);
  }

  main {
    max-width: 880px;
    margin: 0 auto;
  }

  section + section {
    margin-top: 48px;
  }

  .eyebrow {
    font-family: var(--font-mono);
    font-size: 12px;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--text-secondary);
    margin: 0 0 6px;
  }

  h2 {
    font-family: var(--font-display);
    font-weight: 600;
    font-size: 28px;
    margin: 0 0 24px;
    letter-spacing: -0.01em;
  }

  .grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 14px;
  }

  .card {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 20px 20px 18px;
    display: flex;
    flex-direction: column;
    gap: 14px;
  }

  .card-top {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .icon-badge {
    width: 38px;
    height: 38px;
    border-radius: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .icon-badge svg {
    width: 18px;
    height: 18px;
  }

  .tag-gold { background: var(--gold-bg); }
  .tag-gold svg { stroke: var(--gold-icon); }
  .tag-purple { background: var(--purple-bg); }
  .tag-purple svg { stroke: var(--purple-icon); }
  .tag-blue { background: var(--blue-bg); }
  .tag-blue svg { stroke: var(--blue-icon); }

  .pill {
    font-family: var(--font-mono);
    font-size: 11px;
    font-weight: 500;
    letter-spacing: 0.02em;
    padding: 3px 9px;
    border-radius: 999px;
  }

  .pill-gold { background: var(--gold-bg); color: var(--gold-text); }
  .pill-purple { background: var(--purple-bg); color: var(--purple-text); }
  .pill-blue { background: var(--blue-bg); color: var(--blue-text); }

  .card-title {
    font-weight: 600;
    font-size: 15px;
    margin: 0;
  }

  .card-sub {
    font-size: 13px;
    color: var(--text-secondary);
    margin: 0;
  }

  .help-list {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }

  .help-row {
    display: flex;
    align-items: center;
    gap: 14px;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 16px 20px;
  }

  .help-row svg {
    width: 20px;
    height: 20px;
    stroke: var(--text-secondary);
    flex-shrink: 0;
  }

  .help-row span {
    font-size: 14.5px;
  }

  @media (max-width: 720px) {
    .grid { grid-template-columns: repeat(2, 1fr); }
  }

  @media (max-width: 480px) {
    .grid { grid-template-columns: 1fr; }
    h2 { font-size: 24px; }
  }
</style>
</head>
<body>
<main>

  <section>
    <p class="eyebrow">Achievements</p>
    <h2>Trophy case</h2>
    <div class="grid">

      <div class="card">
        <div class="card-top">
          <div class="icon-badge tag-gold" aria-hidden="true">
            <svg viewBox="0 0 24 24" fill="none" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M8 21h8M12 17v4M7 4h10v4a5 5 0 0 1-10 0V4Z"/><path d="M17 5h2a2 2 0 0 1 2 2v1a3 3 0 0 1-3 3M7 5H5a2 2 0 0 0-2 2v1a3 3 0 0 0 3 3"/></svg>
          </div>
          <span class="pill pill-gold">1st place</span>
        </div>
        <div>
          <p class="card-title">Winner, IoT project</p>
          <p class="card-sub">ICP CASE 2025</p>
        </div>
      </div>

      <div class="card">
        <div class="card-top">
          <div class="icon-badge tag-purple" aria-hidden="true">
            <svg viewBox="0 0 24 24" fill="none" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="9" y="2" width="6" height="12" rx="3"/><path d="M5 10a7 7 0 0 0 14 0M12 19v3"/></svg>
          </div>
          <span class="pill pill-purple">Speaker</span>
        </div>
        <div>
          <p class="card-title">Best presenter</p>
          <p class="card-sub">ICP CASE 2026</p>
        </div>
      </div>

      <div class="card">
        <div class="card-top">
          <div class="icon-badge tag-gold" aria-hidden="true">
            <svg viewBox="0 0 24 24" fill="none" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="15" r="6"/><path d="M9 4h6l1 6-4 3-4-3 1-6Z"/></svg>
          </div>
          <span class="pill pill-gold">2nd place</span>
        </div>
        <div>
          <p class="card-title">Runner-up</p>
          <p class="card-sub">ICP hackathon 2026</p>
        </div>
      </div>

      <div class="card">
        <div class="card-top">
          <div class="icon-badge tag-gold" aria-hidden="true">
            <svg viewBox="0 0 24 24" fill="none" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="8" r="5"/><path d="M8.5 13 7 22l5-3 5 3-1.5-9"/></svg>
          </div>
          <span class="pill pill-gold">2nd place</span>
        </div>
        <div>
          <p class="card-title">Runner-up</p>
          <p class="card-sub">Digital Rising Creator Award 2026</p>
        </div>
      </div>

      <div class="card">
        <div class="card-top">
          <div class="icon-badge tag-purple" aria-hidden="true">
            <svg viewBox="0 0 24 24" fill="none" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="9" y="2" width="6" height="12" rx="3"/><path d="M5 10a7 7 0 0 0 14 0M12 19v3"/></svg>
          </div>
          <span class="pill pill-purple">Speaker</span>
        </div>
        <div>
          <p class="card-title">Best presenter</p>
          <p class="card-sub">Model United Nations</p>
        </div>
      </div>

      <div class="card">
        <div class="card-top">
          <div class="icon-badge tag-blue" aria-hidden="true">
            <svg viewBox="0 0 24 24" fill="none" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M3 11v2a1 1 0 0 0 1 1h2l4 4V6L6 10H4a1 1 0 0 0-1 1Z"/><path d="M15 8a5 5 0 0 1 0 8M18 5a9 9 0 0 1 0 14"/></svg>
          </div>
          <span class="pill pill-blue">Reach</span>
        </div>
        <div>
          <p class="card-title">185K+ followers</p>
          <p class="card-sub">Tech news page</p>
        </div>
      </div>

    </div>
  </section>

  <section>
    <p class="eyebrow">Open to collaboration</p>
    <h2>Looking for help with</h2>
    <div class="help-list">
      <div class="help-row">
        <svg viewBox="0 0 24 24" fill="none" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="4" width="18" height="6" rx="1.5"/><rect x="3" y="14" width="18" height="6" rx="1.5"/><circle cx="7" cy="7" r=".6" fill="currentColor" stroke="none"/><circle cx="7" cy="17" r=".6" fill="currentColor" stroke="none"/></svg>
        <span>Reviewing backend architecture and API design patterns</span>
      </div>
      <div class="help-row">
        <svg viewBox="0 0 24 24" fill="none" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><rect x="7" y="2" width="10" height="20" rx="2"/><path d="M11 18h2"/></svg>
        <span>Best practices for scaling Flutter apps in production</span>
      </div>
    </div>
  </section>

</main>
</body>
</html>

---

<div align="center">

### Let's Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](#)

</div>
