---
title: Archive
layout: default
---

## Archive

<ul class="postList">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> {{ post.date }}
    </li>
  {% endfor %}
</ul>
