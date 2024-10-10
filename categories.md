---
layout: page
title: 카테고리 목록
permalink: /categories/
---

<h1>카테고리 목록</h1>

{% for category in site.categories %}
  <h2>{{ category[0] }}</h2>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
