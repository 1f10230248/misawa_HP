---
layout: single
title: "活動報告一覧"
permalink: /misawa_HP/activity/
---

## 活動報告一覧

{% assign posts = site.posts | where_exp: "post", "post.categories contains 'activity'" %}

{% for post in posts %}
### [{{ post.title }}]({{ post.url }})
<small>{{ post.date | date: "%Y年%-m月%-d日" }}</small>

{{ post.excerpt }}

---

{% endfor %}
