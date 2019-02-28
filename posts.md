---
bg: "tools.jpg"
layout: page
crawlertitle: "Max Lee's blog"
permalink: /Post
title: "Post"
summary: "Dev Post"
active: Post
---

{% for post in site.posts limit: 5 %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}
