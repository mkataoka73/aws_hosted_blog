---
layout: default
title: "Home"
---

<h1 class="title">{{ site.title }}</h1>

<p class="description">
  En Partance は有志による語学・人文学の勉強会です。
</p>

<h2 class="sub-title">Recent posts</h2>

<ul class="list posts">
  {% for post in site.posts limit:5  %}
    {% unless post.not_to_list %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endunless %}
  {% endfor %}
</ul>
