---
layout: default
title: Posts
---
<h1 class="title">{{ page.title }}</h1>

All the posts.

<ul class="list posts">
{% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
