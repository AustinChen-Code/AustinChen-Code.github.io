---
layout: archive
title: "AtCoder题解"
permalink: /Atcoder/
---

{% assign atcoder_posts = site.categories.Atcoder %}

<h2>📊 统计信息</h2>
<p><strong>总题解篇数</strong>: {{ atcoder_posts | size }}</p>

<h2>📝 题解列表</h2>

<ul>
  {% for post in atcoder_posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>

{% if atcoder_posts.size == 0 %}
<p>暂无题解，敬请期待！</p>
{% endif %}

<style>
.post-date {
    color: #6c757d;
    font-size: 0.9em;
    margin-left: 10px;
}
</style>
