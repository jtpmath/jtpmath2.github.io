---
title: "Blog"
layout: default
nav_order: 2
---

# Blog

Welcome to my blog! Scroll down to read each post.

{% for post in site.blog %}
## [{{ post.title }}]({{ post.url | relative_url }})
**Date:** {{ post.date | date: "%B %d, %Y" }}

{{ post.excerpt }}

[Read more]({{ post.url | relative_url }})
{% endfor %}
