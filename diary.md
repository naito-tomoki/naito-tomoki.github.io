---
layout: default
title: Diary
permalink: /diary/
---

## :: Diary Log ::

日常の雑記ログです。
毎日かけたらいいとなと思ってます。

<ul>
  {% for post in site.posts %}
    {% if post.categories contains 'diary' %}
    <li>
      <font size="2" color="#999">{{ post.date | date: "%Y/%m/%d" }}</font>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endif %}
  {% endfor %}
</ul>