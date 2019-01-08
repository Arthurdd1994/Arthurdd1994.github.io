---
title: Arthur Dickerson
layout: default
---

<title>Arthur Dickerson</title>

{% for post in site.posts %}
  <article class="post">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div class="postDate">
      {{ post.date | date: "%B %-d, %Y" }}
    </div>
    <div class="permaLink">
      <a href="{{ post.url }}">🔗</a>      
    </div>
    {{ post.content }}
  </article>
  <hr>
{% endfor %}
