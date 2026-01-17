---
layout: default
title: Research
permalink: /research/
---

{% assign research_posts = site.posts | where_exp: "post", "post.categories contains 'research'" %}

{% for post in research_posts %}
- **{{ post.date | date: "%Y-%m-%d" }} · {{ post.title }}**  
  [阅读全文]({{ post.url | relative_url }})
{% endfor %}
