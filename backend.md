---
layout: page
title: 백엔드
---

## 데이터베이스

{% assign database_posts = site.backend | where: "category", "database" %}
{% for post in database_posts %}
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p>{{ post.date | date: "%Y-%m-%d" }}</p>
  {% if post.tags %}
    <p>
      {% for tag in post.tags %}
        <span>#{{ tag }} </span>
      {% endfor %}
    </p>
  {% endif %}
{% endfor %}

## 백엔드 엔지니어링

{% assign engineering_posts = site.backend | where: "category", "backend_engineering" %}
{% for post in engineering_posts %}
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p>{{ post.date | date: "%Y-%m-%d" }}</p>
  {% if post.tags %}
    <p>
      {% for tag in post.tags %}
        <span>#{{ tag }} </span>
      {% endfor %}
    </p>
  {% endif %}
{% endfor %}
