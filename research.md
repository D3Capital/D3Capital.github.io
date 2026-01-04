---
layout: page
title: "Research"
---

{% assign items = site.research %}
{{ items | size }}

{% for r in site.research %}
- {{ r.title }} → {{ r.url }}
{% endfor %}
