---
layout: page # 使用 page 布局而不是 home
title: 记录工作生活感悟
---


这里是我的个人空间，我会在这里分享我的想法、项目和学习笔记。

## 最新文章

{% for post in site.posts limit: 5 %}
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <span class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
  <p>{{ post.excerpt }}</p>
{% endfor %}
