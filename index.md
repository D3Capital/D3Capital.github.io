---
layout: home
title: " "
permalink: /
---

<style>
/* --- Home: full-bleed hero + minimal manifesto --- */

/* Remove any layout padding on the home page (theme-dependent) */
.page-content, .wrapper, .container {
  max-width: none !important;
  padding: 0 !important;
  margin: 0 !important;
}

/* HERO */
.hero {
  position: relative;
  width: 100%;
  height: 86vh;
  min-height: 620px;
  overflow: hidden;
  margin: 0;
}

.hero-img {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.hero-overlay {
  position: absolute;
  inset: 0;
  background:
    linear-gradient(90deg, rgba(0,0,0,.55), rgba(0,0,0,.20), rgba(0,0,0,.45));
}

/* Top nav inside hero */
.hero-top {
  position: absolute;
  top: 22px;
  left: 28px;
  right: 28px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  z-index: 3;
}

.hero-brand a{
  text-decoration: none;
  font-size: 20px;
  font-weight: 700;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: rgba(255,255,255,0.96);
}

.hero-links a{
  text-decoration: none;
  margin-left: 22px;
  font-size: 15px;
  font-weight: 650;
  letter-spacing: 0.04em;
  color: rgba(255,255,255,0.92);
  opacity: 0.9;
}
.hero-links a:hover { opacity: 1; }

/* Hero title block */
.hero-text {
  position: absolute;
  left: 28px;
  right: 28px;
  bottom: 64px;
  z-index: 3;
  max-width: 980px;
}

.hero-text h1 {
  margin: 0 0 10px;
  font-size: 56px;
  line-height: 1.06;
  letter-spacing: 0.01em;
  color: rgba(255,255,255,0.98);
}

.hero-text p {
  margin: 0;
  font-size: 18px;
  line-height: 1.6;
  color: rgba(255,255,255,0.86);
}

/* Manifesto block (fix "half-finished" feeling) */
.manifesto {
  max-width: 860px;
  margin: 84px auto 120px;
  padding: 0 24px;
  text-align: center;
}
.manifesto p {
  margin: 0;
  font-size: 16px;
  line-height: 1.95;
  color: rgba(0,0,0,0.62);
}

/* Mobile */
@media (max-width: 720px) {
  .hero { height: 78vh; min-height: 520px; }
  .hero-top { top: 16px; left: 18px; right: 18px; }
  .hero-brand a{ font-size: 18px; }
  .hero-links a{ margin-left: 14px; font-size: 14px; }
  .hero-text { left: 18px; right: 18px; bottom: 44px; }
  .hero-text h1 { font-size: 40px; }
  .hero-text p { font-size: 16px; }
  .manifesto { margin: 64px auto 96px; }
}
</style>

<!-- HERO -->
<section class="hero" aria-label="D3Capital Hero">
  <img class="hero-img" src="/assets/img/hero.jpg" alt="D3Capital Research">
  <div class="hero-overlay"></div>

  <div class="hero-top">
    <div class="hero-brand">
      <a href="/" aria-label="Home">D3CAPITAL</a>
    </div>
    <nav class="hero-links" aria-label="Primary">
      <a href="/research/">Research</a>
      <a href="/about/">About</a>
    </nav>
  </div>

  <div class="hero-text">
    <h1>D3 Capital Research Notes</h1>
    <p>Systematic thinking on markets, capital, and decisions.</p>
  </div>
</section>
<!-- /HERO -->

<!-- MANIFESTO -->
<section class="manifesto" aria-label="Manifesto">
  <p>
    D3Capital is an independent research notebook focused on structural, non-directional return mechanisms.<br>
    We document reusable research logic, validity ranges, and failure conditions.<br>
    No forecasts. No recommendations.
  </p>
</section>
<!-- /MANIFESTO -->