---
layout: archive
title: "洛谷题解"
permalink: /luogu/
---

{% assign luogu_posts = site.categories.luogu %}

<h2>📊 统计信息</h2>
<p><strong>总题解篇数</strong>: {{ luogu_posts | size }}</p>

<h2>📝 题解列表</h2>

<ul>
  {% for post in luogu_posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>

{% if luogu_posts.size == 0 %}
<p>暂无题解，敬请期待！</p>
{% endif %}
