---
layout: page
title: ""
---

# D3Capital · Capital Research

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
[查看全部 Views →](/views/)
