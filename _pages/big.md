---
title: 大事件
layout: archive
permalink: /big/
collection: big
author_profile: true
---

{% for post in site.big %}
  <article>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | truncate: 100 }}</p>
  </article>
{% endfor %}