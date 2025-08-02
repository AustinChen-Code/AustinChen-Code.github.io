---
layout: archive
title: "洛谷题解"
permalink: /luogu/
---

<h2>题解列表</h2>

<ul>
  {% for post in site.categories.luogu %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      ({{ post.date | date: "%Y-%m-%d" }})
    </li>
  {% endfor %}
</ul>
