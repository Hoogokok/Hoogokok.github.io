---
layout: page
title: 카테고리 목록
permalink: /categories/
---

<h1>카테고리 목록</h1>

<h2>백엔드</h2>
<ul>
  {% for post in site.backend %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> ({{ post.category }})</li>
  {% endfor %}
</ul>

<h2>프론트엔드</h2>
<ul>
  {% for post in site.frontend %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> ({{ post.category }})</li>
  {% endfor %}
</ul>

<h2>프로젝트</h2>
<ul>
  {% for post in site.project %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> ({{ post.category }})</li>
  {% endfor %}
</ul>
