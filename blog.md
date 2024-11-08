---
title: "Blog"
layout: default
nav_order: 2
---

# Blog

Welcome to my blog! Scroll down to read each post.

{% for post in paginator.posts %}
## [{{ post.title }}]({{ post.url | relative_url }})
**Date:** {{ post.date | date: "%B %d, %Y" }}

{{ post.content }}

[Read more]({{ post.url | relative_url }})
{% endfor %}

{% if paginator.previous_page %}
  [Previous]({{ paginator.previous_page_path | relative_url }})
{% endif %}
{% if paginator.next_page %}
  [Next]({{ paginator.next_page_path | relative_url }})
{% endif %}
{% for post in site.blog %}
## [{{ post.title }}]({{ post.url | relative_url }})
**Date:** {{ post.date | date: "%B %d, %Y" }}

{{ post.excerpt }}

[Go to Post for Comments]({{ post.url | relative_url }})
{% endfor %}
