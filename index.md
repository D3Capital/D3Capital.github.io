---
layout: page
title: " "
---
<style>
/* Full-bleed hero (Hindenburg-style) */
.hero-wrap{
  position: relative;
  left: 50%;
  right: 50%;
  width: 100vw;
  margin-left: -50vw;
  margin-right: -50vw;
  margin-top: 0;
  margin-bottom: 36px;
}

.hero{
  position: relative;
  height: clamp(360px, 46vw, 520px);
  overflow: hidden;
  border-radius: 0;
}

/* image */
.hero-img{
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
  transform: scale(1.02);
}

/* overlay to ensure text legibility */
.hero-overlay{
  position: absolute;
  inset: 0;
  background:
  linear-gradient(90deg, rgba(0,0,0,.74), rgba(0,0,0,.18), rgba(0,0,0,.60)),
  linear-gradient(180deg, rgba(160,0,0,.18), rgba(0,0,0,0));
}

/* text layer */
.hero-text{
  position: absolute;
  inset: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: clamp(22px, 4vw, 64px);
  max-width: 1100px;
}

/* FORCE white text, override theme */
.hero-text h1{
  color: #fff !important;
  margin: 0 0 12px;
  font-size: clamp(30px, 3.6vw, 48px);
  line-height: 1.08;
  letter-spacing: .02em;
  text-shadow: 0 10px 24px rgba(0,0,0,.55);
}

.hero-text p{
  color: rgba(255,255,255,.90) !important;
  margin: 0;
  font-size: clamp(14px, 1.4vw, 18px);
  line-height: 1.55;
  text-shadow: 0 10px 22px rgba(0,0,0,.45);
}

/* optional: keep your page content from sticking to edges on very wide screens */
@media (min-width: 1400px){
  .hero-text{ padding-left: calc((100vw - 1200px)/2); }
}
/* Hero topbar overlay */
.hero-topbar{
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  z-index: 5;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 28px;
  padding: 18px clamp(18px, 4vw, 56px);
}

.hero-brand a{
  color: rgba(255,255,255,.92) !important;
  text-decoration: none !important;
  font-weight: 600;
  letter-spacing: .02em;
  text-shadow: 0 10px 22px rgba(0,0,0,.45);
}

.hero-nav{
  display: flex;
  gap: 22px;
}

.hero-nav a{
  color: rgba(255,255,255,.88) !important;
  text-decoration: none !important;
  font-weight: 500;
  letter-spacing: .02em;
  padding: 8px 10px;
  border-radius: 10px;
  text-shadow: 0 10px 22px rgba(0,0,0,.45);
}

.hero-nav a:hover{
  background: rgba(255,255,255,.10);
}

/* Move hero text down a bit so it doesn't collide with topbar */
.hero-text{
  padding-top: clamp(64px, 7vw, 96px) !important;
}
/* Hide theme header on homepage only (layout: page) */
header, .site-header, .page-header{
  display: none !important;
}
</style>

<!-- HERO -->
<div class="hero-wrap">
  <div class="hero">
    <img class="hero-img" src="/assets/img/hero.jpg" alt="D3 Capital Research Notes">
    <div class="hero-overlay"></div>

    <!-- hero top bar -->
    <div class="hero-topbar">
      <div class="hero-brand">
        <a href="/" aria-label="D3Capital Home">D3Capital</a>
      </div>

      <nav class="hero-nav" aria-label="Primary">
        <a href="/research/">Research</a>
        <a href="/journal/">Journal</a>
        <a href="/views/">Views</a>
      </nav>
    </div>

    <div class="hero-text">
      <h1>D3 Capital Research Notes</h1>
      <p>Systematic thinking on markets, capital, and decisions.</p>
    </div>
  </div>
</div>
<!-- /HERO -->

## D3Capital · Capital Research

**Systematic Investor · Data-Driven Arbitrage**

> 本站聚焦于 **可复用、可验证、可规模化的收益结构研究**。  
> 不做行情预测，不输出情绪判断，不提供交易建议。

---

## Research Philosophy

- 研究对象：**结构性收益机制（非方向性）**
- 研究目标：明确 *适用区间 / 失效条件 / 风险来源*
- 研究原则：逻辑自洽 > 经验归纳 > 观点表达

---

## Content Structure

### Research
**结构性研究与核心假设**

- 明确问题定义
- 提出可被证伪的假设
- 给出逻辑边界与失效条件

→ [查看全部 Research →](/research/)

---

### Journal
**执行记录与复盘日志**

- 验证研究假设
- 记录执行偏差
- 反向修正研究结论

→ [查看全部 Journal →](/journal/)

---

### Views
**低频结构判断档案**

- 非即时观点
- 只讨论“结构是否成立”
- 明确时间尺度与不适用区间

→ [查看全部 Views →](/views/)

---

## Latest Research

{% assign research_posts = site.posts | where_exp: "post", "post.categories contains 'research'" %}

{% for post in research_posts limit:3 %}
- **{{ post.date | date: "%Y-%m-%d" }} · {{ post.title }}**
  [阅读全文]({{ post.url | relative_url }})
{% endfor %}

---

## Latest Views
{% assign views_posts = site.posts | where_exp: "post", "post.categories contains 'views'" %}
{% for post in views_posts limit:3 %}
- **{{ post.date | date: "%Y-%m-%d" }} · {{ post.title }}**
  [阅读全文]({{ post.url | relative_url }})
{% endfor %}

---

## Latest Journal
{% assign journal_posts = site.posts | where_exp: "post", "post.categories contains 'journal'" %}
{% for post in journal_posts limit:3 %}
- **{{ post.date | date: "%Y-%m-%d" }} · {{ post.title }}**
  [阅读全文]({{ post.url | relative_url }})
{% endfor %}

---


## Usage Notice

本站内容为研究与方法论记录，不构成投资建议。  
所有研究结论均假设读者具备基本金融与风险认知能力。
[查看全部 Views →]
