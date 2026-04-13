---
layout: home
---

# 欢迎来到我的博客！

这里是我的个人空间，我会在这里分享我的想法、项目和学习笔记。

## 最新文章

{% for post in site.posts limit: 5 %}
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <span class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
  <!-- 只显示摘要，不显示完整内容 -->
  <p>{{ post.excerpt }}</p>
{% endfor %}

<!-- 如果你想完全不显示文章列表，只保留上面的介绍，就把 for 循环部分删掉 -->
