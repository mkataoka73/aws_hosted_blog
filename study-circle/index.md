---
layout: post
title: オンライン勉強会
permalink: /study
---

木曜午前10時〜12時、オンライン勉強会をしています。
内容は以下の二本立てです。

- [ギリシャ語勉強会](/greek)...古典ギリシャ語を勉強する会です
- [読書会](/reading)...哲学書や人文書の読書会です

## Session logs

<ul class="list posts">
  {% for post in site.posts limit:5  %}
    {% unless post.not_to_list %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endunless %}
  {% endfor %}
</ul>
