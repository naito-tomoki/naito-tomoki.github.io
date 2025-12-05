---
layout: default
title: Past Logs
permalink: /log/
---

## :: Past Logs ::

過去の全記事ログです。

<div style="font-family: 'MS PGothic', monospace; font-size:12px;">
  <ul>
    {% for post in site.posts %}
      <li style="margin-bottom:5px; border-bottom:1px dotted #333;">
        <font color="#999">{{ post.date | date: "%Y/%m/%d" }}</font> 
        <span style="color:#666;">[{{ post.categories | join: ', ' }}]</span>
        <br>
        <a href="{{ post.url }}"><b>{{ post.title }}</b></a>
      </li>
    {% endfor %}
  </ul>
</div>
