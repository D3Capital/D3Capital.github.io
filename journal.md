---
layout: page
title: Journal
permalink: /journal/
---

{% assign items = site.categories.journal %}
{% if items and items.size > 0 %}
<ul>
  {% for post in items %}
    <li>
      {{ post.date | date: "%Y-%m-%d" }} ·
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
{% else %}
<p>暂无 Journal 记录。</p>
{% endif %}
