---
layout: archive
title: "Codeforces题解"
permalink: /Codeforces/
---

{% assign codeforces_posts = site.categories.Codeforces %}

<h2>📊 统计信息</h2>
<p><strong>总题解篇数</strong>: {{ codeforces_posts | size }}</p>

<h2>📝 题解列表</h2>

<ul>
  {% for post in codeforces_posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>

{% if codeforces_posts.size == 0 %}
<p>暂无题解，敬请期待！</p>
{% endif %}

<style>
.post-date {
    color: #6c757d;
    font-size: 0.9em;
    margin-left: 10px;
}
</style>
