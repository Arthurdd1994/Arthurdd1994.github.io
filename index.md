---
title: 
layout: default
---

{% for post in site.posts %}
  <article class="post">
    <a href="{{ post.url }}">{{ post.title }}</a>
    {{ post.content }}
  </article>
{% endfor %}
