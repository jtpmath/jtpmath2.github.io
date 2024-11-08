---
title: "First Blog Post"
date: 2024-11-08
excerpt: "This is a preview of the first post."
layout: post
permalink: /blog/:title/
---

<div class="post">
## {{ post.title }}
**Date:** {{ post.date | date: "%B %d, %Y" }}
This is the full content of your first post.
</div>

---

<script src="https://utteranc.es/client.js"
    repo="jtpmath/jtpmath.github.io"
    issue-term="pathname"
    theme="github-light"
    crossorigin="anonymous"
    async>
</script>
