---
layout: default
title: Research
permalink: /research/
---

# Research Archive

{% for post in site.posts %}
## {{ post.title }}

<div style="opacity:.65; font-size:14px; margin-top:-6px; margin-bottom:14px;">
  {{ post.date | date: "%Y-%m-%d" }}
</div>

{{ post.excerpt | strip_html | truncate: 220 }}

<div style="margin-top:10px; margin-bottom:26px;">
  <a href="{{ post.url | relative_url }}">Read →</a>
</div>

{% endfor %}