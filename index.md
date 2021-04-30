---
layout: default
title: "Home"
citation: C'est dans cette élan, dans l'obligation de départ, car nous ne pouvons pas faire autrement, dans cette prise et risque, dans le pari du départ, que nous pouvons vivre une vie qui en vaut la peine.
citation_eng: It's in this impetus, in the obligation of leaving, as we cannot do otherwise, in this capturedness and risk, in the bet of depart, that we can live a life worth living.
---

<h1 class="title">{{ site.title }}</h1>

<p class="description citation">
  <i>"...{{ page.citation_eng }}" — J-L. Nancy</i>
</p>

<h2 class="sub-title">Recent posts</h2>

<ul class="list posts">
  {% for post in site.posts limit:5  %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
