---
layout: archive
title: "杂项"
permalink: /Others/  # 注意首字母大写
category: Others     # 与文件夹名完全一致
---

{% for post in site.categories.Others %}
* [{{ post.title }}]({{ post.url }})
{% endfor %}
