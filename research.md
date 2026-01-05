---
layout: page
title: Research
permalink: /research/
---

{% for post in site.categories.research %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
