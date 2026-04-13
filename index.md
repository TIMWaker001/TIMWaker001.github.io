---
layout: home
---

# 欢迎来到我的博客！

这里是我的个人空间，我会在这里分享我的想法、项目和学习笔记。

{% for post in site.posts limit: 5 %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <span class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
  <p>{{ post.excerpt }}</p>
{% endfor %}
