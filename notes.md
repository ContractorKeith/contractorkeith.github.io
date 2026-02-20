---
title: notes
permalink: /blog
---

# notes

eventually i will write some

---

{% for post in site.posts %}
<div class="post-list-item">
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
  <p>{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
</div>
{% endfor %}
