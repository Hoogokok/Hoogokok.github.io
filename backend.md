---
layout: page
title: 백엔드
---

## 데이터베이스

{% for post in site.backend %}
  {% if post.category == "database" %}
    <h3><a href="{{ post.url | remove: '.html' }}">{{ post.title }}</a></h3>
    <p>{{ post.date | date: "%Y-%m-%d" }}</p>
    {% if post.tags %}
      <p>
        {% for tag in post.tags %}
          <span>#{{ tag }} </span>
        {% endfor %}
      </p>
    {% endif %}
  {% endif %}
{% endfor %}

## 백엔드 엔지니어링

{% for post in site.backend %}
  {% if post.category == "backend_engineering" %}
    <h3><a href="{{ post.url | remove: '.html' }}">{{ post.title }}</a></h3>
    <p>{{ post.date | date: "%Y-%m-%d" }}</p>
    {% if post.tags %}
      <p>
        {% for tag in post.tags %}
          <span>#{{ tag }} </span>
        {% endfor %}
      </p>
    {% endif %}
  {% endif %}
{% endfor %}
