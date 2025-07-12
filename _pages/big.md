---
layout: single
title: 大事件
permalink: /big/
author_profile: true
---

{% for post in site.dajishi %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt | strip_html | truncate: 100 }}</p>
{% endfor %}