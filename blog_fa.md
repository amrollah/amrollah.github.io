---
layout: page
type: blog
title: Blog Farsi
lang: fa
order: 2
---

<div class="posts">
  {% for post in site.posts %}
  {% if post.lang == 'fa' %}
  <div class="post">
    <h1 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>

    <span class="post-date">{{ post.date | date_to_string }}</span>

    {{ post.content }}
     <a href="{{ post.url }}#disqus_thread">
نظرات                   </a>
  </div>
  {% endif %}
  {% endfor %}
</div>


