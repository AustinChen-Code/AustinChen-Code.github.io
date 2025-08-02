---
layout: archive
title: "标准模板库"
permalink: /STL/
category: STL
description: "C++ STL 学习笔记与使用技巧"
---

{% assign stl_posts = site.categories.STL %}

<div class="category-header">
  <h1>📚 标准模板库 (STL)</h1>
  <p class="category-description">C++ 标准模板库学习笔记与使用技巧</p>
</div>

<div class="category-stats">
  <h2>📊 统计信息</h2>
  <ul>
    <li><strong>总文章数</strong>: {{ stl_posts | size }}</li>
    <li><strong>最近更新</strong>: 
      {% if stl_posts.size > 0 %}
        {{ stl_posts.last.date | date: "%Y-%m-%d" }}
      {% else %}
        暂无
      {% endif %}
    </li>
    <li><strong>内容分类</strong>: vector, map, set, algorithm等</li>
  </ul>
</div>

<h2>📝 文章列表</h2>

{% if stl_posts.size > 0 %}
<ul class="post-list">
  {% for post in stl_posts %}
    <li>
      <div class="post-title">
        <a href="{{ post.url }}">{{ post.title }}</a>
        <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
      </div>
      {% if post.description %}
      <p class="post-description">{{ post.description }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>
{% else %}
<div class="empty-state">
  <p>🚧 暂无文章，敬请期待！</p>
  <p>正在整理 STL 相关学习资料...</p>
</div>
{% endif %}

<style>
.category-header {
  margin-bottom: 25px;
}
.category-description {
  color: #6c757d;
  font-size: 1.1em;
}
.category-stats {
  background-color: #f8f9fa;
  padding: 20px;
  border-radius: 8px;
  margin-bottom: 30px;
}
.category-stats ul {
  list-style: none;
  padding-left: 0;
  margin-bottom: 0;
}
.category-stats li {
  margin-bottom: 8px;
}
.post-list {
  list-style: none;
  padding-left: 0;
}
.post-list li {
  margin-bottom: 20px;
  padding-bottom: 15px;
  border-bottom: 1px solid #eee;
}
.post-title {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 8px;
}
.post-date {
  color: #6c757d;
  font-size: 0.9em;
}
.post-description {
  color: #495057;
  margin-bottom: 0;
  font-size: 0.95em;
}
.empty-state {
  background-color: #f8f9fa;
  padding: 30px;
  border-radius: 8px;
  text-align: center;
  color: #6c757d;
}
</style>
