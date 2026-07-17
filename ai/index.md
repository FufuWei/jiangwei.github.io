---
layout: default
title: AI
nav_order: 3
---

# AI

人工智能学习笔记，包含大模型应用、提示工程和AI工具使用经验。

## 笔记列表

{% assign pages_list = site.pages | where_exp: "p", "p.path contains 'ai/'" | where_exp: "p", "p.path != 'ai/index.md'" %}
{% for p in pages_list %}
- [{{ p.title }}]({{ p.url | relative_url }})
{% endfor %}

---

> 将你的 AI 笔记 `.md` 文件放到 `ai/` 目录下，文件头加上 front matter 即可自动出现在上方列表中。