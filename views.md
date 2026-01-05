---
layout: page
title: Views
permalink: /views/
---

{% assign views_posts = site.posts | where_exp: "post", "post.categories contains 'views'" %}

{% for post in views_posts %}
- **{{ post.date | date: "%Y-%m-%d" }} · {{ post.title }}**  
  [阅读全文]({{ post.url | relative_url }})
{% endfor %}
