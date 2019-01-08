---
title: Arthur Dickerson
layout: default
---

<title>Arthur Dickerson</title>

{% for post in site.posts %}
  <article class="post">
    {% if post.altURL == null %}
      <h2><a href="{{ post.url }}">{{ post.title }}</a> <a href="{{ post.url }}" class="permaLink">🔗</a></h2>
    {% else %}
      <h2><a href="{{ post.altURL }}">{{ post.title }}</a> <a href="{{ post.url }}" class="permaLink">🔗</a></h2>
    {% endif %}
    <div class="postDate">
      {{ post.date | date: "%B %-d, %Y" }}
    </div>
    {{ post.content }}
  </article>
  <hr>
{% endfor %}
