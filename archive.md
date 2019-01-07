---
title: Archive
layout: default
---

<ul class="postList">
  {% for post in site.posts %}
    <li>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>  {{ post.date | date: "%B %-d, %Y" }}
    </li>
  {% endfor %}
</ul>
