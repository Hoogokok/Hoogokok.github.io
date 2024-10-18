---
layout: category
title: 백엔드
category: backend
---

백엔드 개발에 관한 모든 포스트를 여기서 확인하세요.

## 데이터베이스
{% assign database_posts = site.backend | where: "category", "database" %}
{% for post in database_posts %}
<h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
<p>{{ post.date | date: "%Y-%m-%d" }}</p>
{% endfor %}

## 백엔드 엔지니어링
{% assign engineering_posts = site.backend | where: "category", "backend_engineering" %}
{% for post in engineering_posts %}
<h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
<p>{{ post.date | date: "%Y-%m-%d" }}</p>
{% endfor %}

## Nest.js
{% assign nest_posts = site.backend | where: "category", "nest.js" %}
{% for post in nest_posts %}
<h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
<p>{{ post.date | date: "%Y-%m-%d" }}</p>
{% endfor %}

