---
layout: default
title: 홈
---

개발 요모조모

{% assign all_posts = site.posts | concat: site.backend | concat: site.frontend %}

<h1>최근 게시물</h1>

<ul>
  {% for post in all_posts limit:5 %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.date | date: "%Y-%m-%d" }}</p>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>