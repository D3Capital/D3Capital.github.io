---
layout: home
title: ""
---

<style>
/* ===== Homepage hard reset (remove top white gap) ===== */
html, body { margin: 0 !important; padding: 0 !important; }
body { padding-top: 0 !important; }

/* Hide theme header on homepage (common selectors) */
header,
.site-header,
.page-header,
.masthead,
.navbar {
  display: none !important;
  height: 0 !important;
  margin: 0 !important;
  padding: 0 !important;
}

/* Remove top spacing from common wrappers/containers */
main,
.page-content,
.container,
.wrapper,
.content,
#content {
  margin-top: 0 !important;
  padding-top: 0 !important;
}

/* ===== HERO (full-bleed) ===== */
.hero {
  position: relative;
  width: 100vw;
  margin-left: calc(50% - 50vw);
  margin-right: calc(50% - 50vw);
  height: 72vh;
  min-height: 520px;
  overflow: hidden;
}

.hero-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
  transform: scale(1.01);
}

/* Strong overlay to guarantee readability */
.hero-overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(
    180deg,
    rgba(0,0,0,0.60) 0%,
    rgba(0,0,0,0.35) 45%,
    rgba(0,0,0,0.68) 100%
  );
}

/* Top nav inside hero */
.hero-topbar {
  position: absolute;
  top: 22px;
  left: 42px;
  right: 42px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  z-index: 5;
  font-size: 14px;
  letter-spacing: 0.06em;
}

.hero-brand a {
  color: rgba(255,255,255,0.96) !important;
  text-decoration: none !important;
  font-weight: 700;
  font-size: 18px;          /* 核心调整点 */
  letter-spacing: 0.04em;   /* 机构感 */
  text-transform: uppercase; /* 可选，偏机构 */
  text-shadow: 0 12px 26px rgba(0,0,0,0.55);
}

.hero-links {
  display: flex;
  gap: 22px;
}

.hero-links a {
  color: rgba(255,255,255,0.85) !important;
  text-decoration: none !important;
  font-size: 16px;
  font-weight: 400;
  letter-spacing: 0.06em;
  padding: 8px 10px;
  border-radius: 10px;
  text-shadow: 0 10px 22px rgba(0,0,0,0.45);
}

.hero-links a:hover {
  background: rgba(255,255,255,0.10);
  color: #fff !important;
}

/* Hero title block */
.hero-text {
  position: absolute;
  left: 42px;
  right: 42px;
  bottom: 88px;
  max-width: 980px;
  z-index: 4;
}

.hero-text h1 {
  color: #fff !important;
  margin: 0 0 12px;
  font-size: clamp(30px, 3.6vw, 48px);
  font-weight: 500;
  letter-spacing: 0.02em;
  line-height: 1.12;
  text-shadow: 0 10px 24px rgba(0,0,0,0.55);
}

.hero-text p {
  color: rgba(255,255,255,0.90) !important;
  margin: 0;
  font-size: clamp(14px, 1.35vw, 18px);
  line-height: 1.55;
  text-shadow: 0 10px 22px rgba(0,0,0,0.45);
}

/* Mobile */
@media (max-width: 768px) {
  .hero { height: 60vh; min-height: 420px; }
  .hero-topbar { left: 18px; right: 18px; top: 16px; }
  .hero-text { left: 18px; right: 18px; bottom: 44px; }
}
.hero-top {
  position: absolute;
  top: 28px;
  left: 32px;
  right: 32px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 5;
}

.hero-brand {
  font-size: 18px;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: rgba(255,255,255,0.95);
  text-decoration: none;
}

.hero-links a {
  margin-left: 28px;
  font-size: 15px;
  font-weight: 500;
  letter-spacing: 0.04em;
  color: rgba(255,255,255,0.9);
  text-decoration: none;
}

.hero-links a:hover {
  opacity: 1;
}
</style>

<!-- HERO -->
<section class="home-statement">
  <p>
    D3Capital is an independent research notebook.<br>
    We focus on structural, non-directional return mechanisms.<br>
    No forecasts. No recommendations.
  </p>
</section>

<style>
.home-statement{
  padding: 72px 24px 120px;
  text-align: center;
  color: #666;
  font-size: 14px;
  line-height: 1.9;
}
</style>
<div class="hero">
  <div class="hero-top">
  <a class="hero-brand" href="/">D3Capital</a>

  <nav class="hero-links">
    <a href="/research/">Research</a>
    <a href="/about/">About</a>
  </nav>
</div>
  <img class="hero-img" src="/assets/img/hero.jpg" alt="D3Capital Research">
  <div class="hero-overlay"></div>

  <div class="hero-topbar">
    <div class="hero-brand">
      <a href="/" aria-label="D3Capital Home">D3Capital</a>
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
</div>
<!-- /HERO -->