---
layout: default
title: AIニュース記事
---

# AI関連のニュース記事

{% assign posts = site.posts %}

{% if posts.size > 0 %}
{% for post in posts %}

## [{{ post.title }}]({{ post.url | relative_url }})

📅 {{ post.date | date: "%Y-%m-%d" }}

{{ post.excerpt }}

---

{% endfor %}
{% else %}

まだ記事はありません。

{% endif %}
