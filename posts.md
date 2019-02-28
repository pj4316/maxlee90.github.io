---
bg: "tools.jpg"
layout: default
crawlertitle: "Max Lee's blog"
title: "Max Lee - Dev Post"
summary: "Dev Post"
---

{% for post in site.posts limit: 10 %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}
