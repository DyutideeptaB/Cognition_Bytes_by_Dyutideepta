---
layout: home
title: Blog
permalink: /blog/
---

<ul>
{% for post in site.posts %}
  <li>
    <strong>{{ post.date | date: "%b %d, %Y" }}</strong> — 
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

