---
title: Archive
layout: default
---

{% for post in site.posts %}
  <article class="post">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div class="postDate">
      {{ post.date | date: "%B %-d, %Y" }}
    </div>
    {{ post.excerpt }}
    <a href="{{ post.url }}">Read more...</a>
  </article>
  <hr>
{% endfor %}
