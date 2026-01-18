---
layout: default
title: Research
permalink: /research/
---

# Research Archive

{% for post in site.posts %}
## {{ post.title }}

<div style="opacity:.6; font-size:13px; margin-top:-10px; margin-bottom:14px;">
  {{ post.date | date: "%Y-%m-%d" }}
</div>

{{ post.excerpt | strip_html | truncate: 220 }}

<div style="margin-top:10px; margin-bottom:30px;">
  <a href="{{ post.url | relative_url }}">Read →</a>
</div>
{% endfor %}