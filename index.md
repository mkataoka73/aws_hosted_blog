---
layout: default
title: "Home"
---

<h1 class="title">{{ site.title }}</h1>

<p class="description">{{ site.description }}</p>

<h2 class="sub-title">Recent posts</h2>

<ul class="posts">
  {% for post in site.posts %}
    <li class="post-li">
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
