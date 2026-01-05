---
layout: page
title: Journal
permalink: /journal/
---

{% assign journal_posts = site.posts | where_exp: "post", "post.categories contains 'journal'" %}

{% for post in journal_posts %}
- **{{ post.date | date: "%Y-%m-%d" }} · {{ post.title }}**  
  [阅读全文]({{ post.url | relative_url }})
{% endfor %}
