---
layout: default
title: 专业
nav_order: 2
---

# 专业

技术专业能力沉淀，包含架构设计、最佳实践和问题排查经验。

## 笔记列表

{% assign pages_list = site.pages | where_exp: "p", "p.path contains 'professional/'" | where_exp: "p", "p.path != 'professional/index.md'" %}
{% for p in pages_list %}
- [{{ p.title }}]({{ p.url | relative_url }})
{% endfor %}

---

> 将你的专业笔记 `.md` 文件放到 `professional/` 目录下，文件头加上 front matter 即可自动出现在上方列表中。