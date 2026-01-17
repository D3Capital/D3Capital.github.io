---
layout: home
title: ""
---

<style>
/* ========== HERO BASE ========== */
.hero {
  position: relative;
  width: 100%;
  height: clamp(640px, 92vh, 860px);
  overflow: hidden;
}

/* Background image */
.hero-img {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* Dark overlay */
.hero-overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(
    180deg,
    rgba(0,0,0,0.55) 0%,
    rgba(0,0,0,0.35) 40%,
    rgba(0,0,0,0.55) 100%
  );
}

/* Top navigation inside hero */
.hero-top {
  position: absolute;
  top: 28px;
  left: 40px;
  right: 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 5;
}

.hero-brand {
  font-size: 22px;
  font-weight: 600;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: rgba(255,255,255,0.95);
  text-decoration: none;
  text-shadow: 0 2px 10px rgba(0,0,0,0.35);
}

.hero-links a {
  margin-left: 32px;
  font-size: 17px;
  font-weight: 500;
  letter-spacing: 0.05em;
  color: rgba(255,255,255,0.9);
  text-decoration: none;
  text-shadow: 0 2px 10px rgba(0,0,0,0.35);
}

.hero-links a:hover {
  opacity: 1;
}

/* Center text */
.hero-text {
  position: relative;
  z-index: 4;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding-left: 64px;
  max-width: 900px;
}

.hero-text h1 {
  margin: 0 0 14px;
  font-size: 48px;
  line-height: 1.15;
  font-weight: 600;
  color: #fff;
  text-shadow: 0 2px 10px rgba(0,0,0,0.35);
}

.hero-text p {
  margin: 0;
  font-size: 18px;
  line-height: 1.6;
  color: rgba(255,255,255,0.9);
}

/* Mobile */
@media (max-width: 768px) {
  .hero-text {
    padding-left: 28px;
    padding-right: 28px;
  }
  .hero-text h1 {
    font-size: 34px;
  }
  .hero-top {
    left: 20px;
    right: 20px;
  }
}
</style>

<div class="hero">
  <img class="hero-img" src="/assets/img/hero.jpg" alt="D3 Capital Research">
  <div class="hero-overlay"></div>

  <div class="hero-top">
    <a class="hero-brand" href="/">D3Capital</a>
    <nav class="hero-links">
      <a href="/research">Research</a>
      <a href="/about">About</a>
    </nav>
  </div>

  <div class="hero-text">
    <h1>D3 Capital Research Notes</h1>
    <p>Systematic thinking on markets, capital, and decisions.</p>
  </div>
</div>