---
layout: category
title: 백엔드
category: backend
---

백엔드 개발에 관한 모든 포스트를 여기서 확인하세요.

{% for post in site.backend %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: "%Y-%m-%d" }}</p>
  <p>{{ post.excerpt }}</p>
{% endfor %}
