---
layout: page
title: ""
permalink: /blog/
---

# 📚 View my Blogs

{% for post in site.posts %}
- **{{ post.date | date: "%b %d, %Y" }}** — [{{ post.title }}]({{ post.url }})
{% endfor %}

📬 **Subscribe to my blog via email**:  
[Click here to get new posts updates directly in your inbox](https://blogtrottr.com/?subscribe=http://dyutideepta.is-a.dev/feed.xml)

