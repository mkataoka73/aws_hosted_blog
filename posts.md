---
layout: default
title: posts
---
<h1 class="title">Posts</h1>

uncategorizedな記事たち

<ul class="list posts">
  {% for post in site.posts | where: "category", "journal" %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
