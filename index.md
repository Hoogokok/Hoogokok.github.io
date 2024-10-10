---
layout: default
title: 홈
---

개발 요모조모

## 최근 포스트

{% assign all_posts = site.backend | concat: site.frontend | concat: site.devops %}
{% assign sorted_posts = all_posts | sort: 'date' | reverse %}

{% for post in sorted_posts limit:5 %}
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p>{{ post.excerpt }}</p>
{% endfor %}

## 카테고리

- [백엔드](/backend)
- [프론트엔드](/frontend)

