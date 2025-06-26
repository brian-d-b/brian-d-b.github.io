---
layout: default
title: Home
---

# My Notes

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a><br>
    <small>{{ post.date | date: "%B %d, %Y" }}</small><br>
    <p>{{ post.excerpt }}</p>
  </li>
{% endfor %}
</ul>
