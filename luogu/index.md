---
layout: archive
title: "洛谷题解"
permalink: /luogu/
---

<h2>📊 统计信息</h2>
<p><strong>总题解篇数</strong>: {% raw %}{{ site.categories.luogu | size }}{% endraw %}</p>

<h2>📝 题解列表</h2>

<ul>
  {% raw %}{% for post in site.categories.luogu %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      ({{ post.date | date: "%Y-%m-%d" }})
    </li>
  {% endfor %}{% endraw %}
</ul>
