---
layout: page
title: 백엔드
---

## 데이터베이스

{% for post in site.backend %}
  {% if post.path contains '/database/' %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p>{{ post.date | date: "%Y-%m-%d" }}</p>
    {% if post.excerpt %}
      <p>{{ post.excerpt }}</p>
    {% endif %}
  {% endif %}
{% endfor %}

## 백엔드 엔지니어링

{% for post in site.backend %}
  {% if post.path contains '/engineering/' %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p>{{ post.date | date: "%Y-%m-%d" }}</p>
    {% if post.excerpt %}
      <p>{{ post.excerpt }}</p>
    {% endif %}
  {% endif %}
{% endfor %}
