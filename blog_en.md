---
layout: page
type: blog
title: Blog English
lang: en
order: 1
icon: flaticon-globe35
---

<div class="posts">
  {% for post in site.posts %}
  {% if post.lang == page.lang %}
  <div class="post">
    <h1 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>

    <span class="post-date">{{ post.date | date_to_string }}</span>

    {{ post.content }}
    {% if site.comments %}
     <a href="{{ post.url }}#disqus_thread">
           comments    </a>
           {% endif %}
  </div>
  {% endif %}
  {% endfor %}
</div>



