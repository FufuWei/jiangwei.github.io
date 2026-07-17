---
layout: default
title: 业务
nav_order: 1
---

# 业务

业务领域知识沉淀，包含项目经验、业务流程梳理和复盘总结。

## 笔记列表

{% assign pages_list = site.pages | where_exp: "p", "p.path contains 'business/'" | where_exp: "p", "p.path != 'business/index.md'" %}
{% for p in pages_list %}
- [{{ p.title }}]({{ p.url | relative_url }})
{% endfor %}

---

> 将你的业务笔记 `.md` 文件放到 `business/` 目录下，文件头加上 front matter 即可自动出现在上方列表中。