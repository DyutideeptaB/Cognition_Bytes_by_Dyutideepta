---
layout: page
title: ""
permalink: /blog/
---

# 📚 View my Blogs

{% for post in site.posts %}
- **{{ post.date | date: "%b %d, %Y" }}** — [{{ post.title }}]({{ post.url }})
{% endfor %}

<a href="https://blogtrottr.com/?subscribe=http://dyutideepta.is-a.dev/feed.xml" target="_blank">
  📬 Subscribe via Email
</a>

