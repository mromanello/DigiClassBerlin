---
layout: default
title: Blog
---
{% for post in site.posts limit:5 %}
  <div class="item">
    <div class="item_details">
      <h2>{{ post.title }}</h2>
      <h3>Posted on <a href="/berlin{{ post.url }}" title="Permalink for this post">{{ post.date | date_to_string }}</a></h3>
    </div>
    <div class="item_content">
      {{ post.content }}
    </div>
  </div>
  {% endfor %}