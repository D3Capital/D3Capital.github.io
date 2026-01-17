---
layout: page
title: ""
---

<style>
/* ===== HERO LAYOUT ===== */
.hero {
  position: relative;
  width: 100vw;
  margin-left: calc(50% - 50vw);
  margin-right: calc(50% - 50vw);
  height: 72vh;
  min-height: 520px;
  overflow: hidden;
}

/* Background image */
.hero-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

/* Dark overlay for text contrast */
.hero-overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(
    180deg,
    rgba(0,0,0,0.55) 0%,
    rgba(0,0,0,0.35) 40%,
    rgba(0,0,0,0.65) 100%
  );
}

/* Top navigation inside hero */
.hero-nav {
  position: absolute;
  top: 28px;
  left: 48px;
  right: 48px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 3;
  font-size: 14px;
  letter-spacing: 0.06em;
}

.hero-nav a {
  color: rgba(255,255,255,0.85);
  text-decoration: none;
  margin-left: 28px;
}

.hero-nav a:hover {
  color: #ffffff;
}

/* Hero text */
.hero-text {
  position: absolute;
  left: 48px;
  bottom: 96px;
  max-width: 820px;
  color: #ffffff;
  z-index: 2;
}

.hero-text h1 {
  margin: 0 0 14px;
  font-size: 46px;
  font-weight: 500;
  letter-spacing: 0.02em;
  line-height: 1.15;
}

.hero-text p {
  margin: 0;
  font-size: 18px;
  line-height: 1.6;
  opacity: 0.9;
}

/* Mobile */
@media (max-width: 768px) {
  .hero {
    height: 60vh;
    min-height: 420px;
  }
  .hero-text {
    left: 22px;
    right: 22px;
    bottom: 48px;
  }
  .hero-text h1 {
    font-size: 32px;
  }
}
</style>

<!-- HERO -->
<div class="hero">
  <img class="hero-img" src="/assets/img/hero.jpg" alt="D3Capital Research">
  <div class="hero-overlay"></div>

  <div class="hero-nav">
    <div class="hero-brand">
      <a href="/">D3Capital</a>
    </div>
    <div class="hero-links">
      <a href="/research/">Research</a>
      <a href="/journal/">Journal</a>
      <a href="/views/">Views</a>
    </div>
  </div>

  <div class="hero-text">
    <h1>D3 Capital Research Notes</h1>
    <p>Systematic thinking on markets, capital, and decisions.</p>
  </div>
</div>
<!-- /HERO -->

<br>

D3Capital documents research on structural, non-directional return mechanisms.

We focus on repeatable, falsifiable strategies across markets and capital structures.  
No market forecasts. No investment advice.

<br>

For professional or research-related correspondence:  
data3capital@outlook.com