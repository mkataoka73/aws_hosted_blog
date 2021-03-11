---
layout: default
title: "Home"
---

<h1 class="title">プログラミングの学び方</h1>

<p class="description">ノンプログラマである30ぐらいの小さな塾勤めの若造が、呑気に気ままに、時にあくせく、プログラミングの学習日記をつけていくサイトです。</p>

<h2 class="sub-title">Recent posts</h2>

<ul class="posts">
  {% for post in site.posts %}
    <li class="post-li">
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
