---
bg: "tools.jpg"
layout: default
crawlertitle: "Max Lee's blog"
permalink: /Post/
title: "Post"
summary: "Dev Post"
active: Post
---

<li><a href="/Post/">Post</a>
  <ul>
      <li><a href="/Post/EJ/0">Effective Java</a></li>
  </ul>
  <ul>
      <li><a href="/Post/Gradle/0">Gradle</a></li>
  </ul>
</li>

{% for post in site.posts limit: 5 %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}
