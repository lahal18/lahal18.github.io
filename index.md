---
layout: default
title: Welcome to My Tech Blog
---

# Welcome to My Blog!

This is where I share the latest insights on technology, AI, and programming, all generated with the help of my automation bot.

---

## Latest Posts

{% for post in site.posts %}
  <article>
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p><small>Published on: {{ post.date | date: "%B %d, %Y" }}</small></p>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}