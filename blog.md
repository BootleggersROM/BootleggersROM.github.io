---
layout: default
title: Blog
excerpt_separator: <!--morepost-->
---
{% for post in site.posts %}
  <div class="card shishu-light-bg z-depth-3">
    <div class="card-image">
      <img src="{{ post.image }}" style="max-height:300px">
      <span class="card-title">{{ post.title }}</span>
    </div>
    <div class="card-content">
      {{ post.excerpt }}
    </div>
    <div class="card-action">
      <a href="{{ post.url }}">Read more</a>
    </div>
  </div>
  <br>
{% endfor %}
