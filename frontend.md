---
layout: category
title: 프론트엔드
category: frontend
---

프론트엔드 개발에 관한 모든 포스트를 여기서 확인하세요.
## 프론트엔드 잡답
{% assign frontend_posts = site.frontend | where: "category", "frontend_about" %}
{% for post in frontend_posts %}
<h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
<p>{{ post.date | date: "%Y-%m-%d" }}</p>
{% endfor %}
