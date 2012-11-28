---
layout: default
title: Blog
---
{% for post in site.posts limit:5 %}
  <div class="item">
    <div class="item_details">
      <h2><a href="/berlin{{ post.url }}" title="Permalink for this post">{{ post.title }}</a></h2>
      <h3>Posted on {{ post.date | date_to_string }}</h3>		
    </div>
<!--
    <div class="item_content">
      {{ post.content }}
    </div>-->
  </div>
  {% endfor %}