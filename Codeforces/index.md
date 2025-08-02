---
layout: archive
title: "Codeforces题解"
permalink: /Codeforces/  # 注意首字母大写
category: Codeforces     # 与文件夹名完全一致
---

<h2>题解列表</h2>

<ul>
  {% for post in site.categories.Codeforces %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      ({{ post.date | date: "%Y-%m-%d" }})
    </li>
  {% endfor %}
</ul>
