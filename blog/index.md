---
layout: page
title: Blog
permalink: /blog/
---

# 📚 Blog Posts

{% for post in site.posts %}
- **{{ post.date | date: "%b %d, %Y" }}** — [{{ post.title }}]({{ post.url }})
{% endfor %}

