---
layout: page
title: Views
permalink: /views/
---

{% assign items = site.categories.views %}
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
<p>暂无 Views 文章。</p>
{% endif %}
