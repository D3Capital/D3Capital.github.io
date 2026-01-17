---
layout: page
title: ""
permalink: /
---
<style>
/* --- Home: full-bleed hero + tight manifesto --- */

/* Kill layout spacing on HOME only (safer) */
body.home .page-content,
body.home .wrapper,
body.home .container{
  max-width: none !important;
  padding: 0 !important;
  margin: 0 !important;
}

/* Remove theme header spacing on HOME (this fixes the top white bar) */
body.home .site-header,
body.home .topbar{
  display: none !important;
}

/* HERO */
.hero{
  position: relative;
  width: 100%;
  height: 74vh;
  min-height: 520px;
  overflow: hidden;
  margin: 0;
}

.hero-img{
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.hero-overlay{
  position: absolute;
  inset: 0;
  background: linear-gradient(90deg, rgba(0,0,0,.58), rgba(0,0,0,.20), rgba(0,0,0,.50));
}

/* Top nav inside hero */
.hero-top{
  position: absolute;
  top: 18px;
  left: 24px;
  right: 24px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  z-index: 3;
}

.hero-brand a{
  text-decoration: none;
  font-size: 22px;
  font-weight: 750;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: rgba(255,255,255,0.96);
}

.hero-links a{
  text-decoration: none;
  margin-left: 22px;
  font-size: 16px;
  font-weight: 650;
  letter-spacing: 0.04em;
  color: rgba(255,255,255,0.92);
  opacity: 0.92;
}
.hero-links a:hover{ opacity: 1; }

/* Title block */
.hero-text{
  position: absolute;
  left: 24px;
  right: 24px;
  top: 56%;
  transform: translateY(-50%);
  z-index: 3;
  max-width: 980px;
}

.hero-text h1{
  margin: 0 0 10px;
  font-size: 56px;
  line-height: 1.06;
  letter-spacing: 0.01em;
  color: rgba(255,255,255,0.98);
}

.hero-text p{
  margin: 0;
  font-size: 18px;
  line-height: 1.6;
  color: rgba(255,255,255,0.86);
}

/* Manifesto: tight and clean */
.manifesto{
  max-width: 880px;
  margin: 14px auto 32px;   /* tighter: removes the “half-finished” feel */
  padding: 0 24px;
  text-align: center;
}
.manifesto p{
  margin: 0;
  font-size: 15px;
  line-height: 1.85;
  color: rgba(0,0,0,0.62);
}
.manifesto .manifesto-link{
  margin-top: 10px;
  font-size: 13px;
  opacity: .55;
}
.manifesto a{
  color: inherit;
  text-decoration: underline;
  text-underline-offset: 3px;
}

/* Mobile */
@media (max-width: 720px){
  .hero{ height: 68vh; min-height: 480px; }
  .hero-top{ top: 14px; left: 16px; right: 16px; }
  .hero-brand a{ font-size: 19px; }
  .hero-links a{ margin-left: 14px; font-size: 14px; }
  .hero-text{ left: 16px; right: 16px; top: 62%; }
  .hero-text h1{ font-size: 40px; }
  .hero-text p{ font-size: 16px; }
  .manifesto{ margin: 12px auto 26px; }
}
</style>

<!-- HERO -->
<section class="hero" aria-label="D3Capital Hero">
  <img class="hero-img" src="{{ '/assets/img/hero.jpg' | relative_url }}" alt="D3Capital Research">
  <div class="hero-overlay"></div>

  <div class="hero-top">
    <div class="hero-brand">
      <a href="{{ '/' | relative_url }}" aria-label="Home">D3CAPITAL</a>
    </div>
    <nav class="hero-links" aria-label="Primary">
      <a href="{{ '/research/' | relative_url }}">Research</a>
      <a href="{{ '/about/' | relative_url }}">About</a>
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
  <p class="manifesto-link">
    Selected research is available under <a href="{{ '/research/' | relative_url }}">Research</a>.
  </p>
</section>
<!-- /MANIFESTO -->
