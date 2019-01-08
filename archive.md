---
title: Archive
layout: default
---

{% for post in site.posts %}
  <article class="post">
    {% if post.altURL == null %}
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    {% else %}
      <h2><a href="{{ post.altURL }}">{{ post.title }}</a></h2>
    {% endif %}
    <div class="permaLink">
      <a href="{{ post.url }}">🔗</a>      
    </div>
    <div class="postDate">
      {{ post.date | date: "%B %-d, %Y" }}
    </div>
    {{ post.excerpt }}
    <a href="{{ post.url }}">Read more...</a>
  </article>
  <hr>
{% endfor %}
