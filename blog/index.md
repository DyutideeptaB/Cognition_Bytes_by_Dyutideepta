---
layout: page
title: ""
permalink: /blog/
---

# 📚 View my Blogs

{% for post in site.posts %}
- **{{ post.date | date: "%b %d, %Y" }}** — [{{ post.title }}]({{ post.url }})
{% endfor %}

