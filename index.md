---
layout: default
title: "Home"
---

# プログラミングの学び方
{:.title}

## 語学の記録とTechの関連
{:.sub-title}

ノンプログラマである30ぐらいの小さな塾勤めの若造が、呑気に気ままに、時にあくせく、プログラミングの学習日記をつけていくサイトです。
{:.description}

## Recent posts
{:.sub-title}


{% for post in site.posts %}
  - [{{ post.title }}]({{ post.url }}){:.post-li}
{% endfor %}
