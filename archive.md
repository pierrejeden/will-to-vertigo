---
title: Archive
layout: default
permalink: /archive/
---

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url | relative_url }})

{{ post.date | date: "%Y-%m-%d" }}{% if post.lang %} · {{ post.lang }}{% endif %}
{% endfor %}
