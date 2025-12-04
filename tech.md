---
layout: default
title: Tech Notes
permalink: /tech/
---

## :: Tech Notes ::

C言語、Linux、アルゴリズムなどの技術メモ（にする予定）。

<ul>
  {% for post in site.posts %}
    {% if post.categories contains 'tech' %}
    <li>
      <font size="2" color="#999">{{ post.date | date: "%Y/%m/%d" }}</font>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endif %}
  {% endfor %}
</ul>