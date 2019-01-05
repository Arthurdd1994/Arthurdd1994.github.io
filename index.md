---
title: 
layout: default
---

<title>Arthur Dickerson</title>

{% for post in site.posts %}
  <article class="post">
    <a href="{{ post.url }}">{{ post.title }}</a>
    {{ post.content }}
  </article>
{% endfor %}
