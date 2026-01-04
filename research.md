---
layout: page
title: Research
permalink: /research/
---

{% assign items = site.categories.research %}
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
<p>暂无 Research 文章。</p>
{% endif %}
