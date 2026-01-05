---
layout: page
title: ""
permalink: /
---

## D3Capital · Capital Research

**Systematic Investor · Data-Driven Arbitrage**

本站专注于研究**可复用、可验证、可规模化的收益结构**，  
不做行情预测，不输出情绪判断。

---

## 研究站规则

- **Research**：结构性研究与核心假设，强调逻辑自洽与边界条件  
- **Journal**：执行记录与复盘日志，用于验证研究与修正偏差  
- **Views**：低频结构判断，明确适用区间与失效条件

---

## 最新更新

### Research
{% for post in site.categories.research limit: 5 %}
- {{ post.date | date: "%Y-%m-%d" }} · [{{ post.title }}]({{ post.url }})
{% endfor %}
[查看全部 Research →](/research/)

---

### Journal
{% for post in site.categories.journal limit: 5 %}
- {{ post.date | date: "%Y-%m-%d" }} · [{{ post.title }}]({{ post.url }})
{% endfor %}
[查看全部 Journal →](/journal/)

---

### Views
{% for post in site.categories.views limit: 5 %}
- {{ post.date | date: "%Y-%m-%d" }} · [{{ post.title }}]({{ post.url }})
{% endfor %}
[查看全部 Views →](/views/)
