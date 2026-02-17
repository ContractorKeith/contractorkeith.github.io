---
title: Blog
permalink: /blog
---

# Blog

Notes on construction tech, estimating tools, and what I'm learning.

---

{% for post in site.posts %}
<div class="post-list-item">
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
  <p>{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
</div>
{% endfor %}
