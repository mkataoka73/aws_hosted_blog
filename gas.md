---
layout: default
title: GAS
---
<h1 class="title">{{ page.title }}</h1>

GAS articles

<ul class="list posts">
  {% assign posts = site.posts | where: "categories", "gas" %}
  {% for post in posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
