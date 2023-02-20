---
title: Post
layout: posts
description: Post
permalink: "/post/"
intro_image_absolute: true
intro_image_hide_on_mobile: false
paginate: 3
---

# Aprende más

Te muestro algunas prácticas que hemos hecho a lo largo del curso



{% for post in site.posts %}
  <div class="post">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.date | date_to_string }}</p>
    <div class="post-content">{{ post.content | truncate: 120 }}</div>
    <a href="{{ post.url }}">Read more</a>
  </div>
{% endfor %}