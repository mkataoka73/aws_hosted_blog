---
layout: default
title: posts
---
<h1 class="title">Posts</h1>

<ul class="posts">
  {% for post in site.posts %}
    <li class="post-li">
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
