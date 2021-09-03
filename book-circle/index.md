---
layout: default
title: 読書会
permalink: /reading
text_name: Being Ecological
text_url: https://www.amazon.co.jp/dp/B077T848F8/
test: {{ site.title }}
---

# {{ page.title }}
{:.title}

哲学書を読む会です。

今は Timothy Morton の Being Ecological を読んでいます。


## 概要

| 内容   | 哲学を勉強する会 |
| 教科書   | [{{ page.text_name }}]({{ page.text_url }}){:target="_blank"} |
| 日時 | 毎月第2・第4木曜日　10:00~12:00                                            |
| 場所     | Zoom                        |
| 参加費     | 無料                        |
{:.table}


- 開催日時は、時々変更の可能性があります。
- 人数が増えたら、Zoom以外のソフトに切り替えるかもしれません。

## 読みたい本リスト

<ul>
{% for book in site.data.books %}
  <li>
    <a href="{{ book.page_link }}">
      {{ book.title }}
    </a>
    {% if book.now_reading %}
      <span>— Now Reading</span>
    {% endif %}
  </li>
{% endfor %}
</ul>
