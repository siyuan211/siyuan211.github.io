---
layout: single
title: 大事件
permalink: /big/
author_profile: true
---

<h1>大事件目录</h1>

<ul>
  {% for post in site.dajishi %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}</li>
  {% endfor %}
</ul>