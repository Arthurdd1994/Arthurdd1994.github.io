---
title: Arthur Dickerson
layout: default
---

<title>Arthur Dickerson</title>

{% for post in site.posts %}
  <article class="post">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    {{ post.content }}
  </article>
  <hr>
{% endfor %}
