---
layout: page
title: Research
---

# Research Archive

{% for post in site.posts %}
## {{ post.title }}

<div style="opacity:.55; font-size:14px; margin-top:-8px; margin-bottom:14px;">
  {{ post.date | date: "%Y-%m-%d" }}
</div>

{{ post.excerpt | strip_html | truncate: 220 }}

<div style="margin-top:12px; margin-bottom:36px;">
  <a href="{{ post.url | relative_url }}">Read →</a>
</div>

{% endfor %}