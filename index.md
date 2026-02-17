---
title: Home
permalink: /
---

# Welcome

I'm Keith — a fence estimator at Complete Custom Fence in Central Florida with 35+ years in the construction industry. I'm building internal tools to streamline my estimating workflow and documenting the process here.

## What You'll Find Here

- **[Projects](/projects)** — Tools and repos I'm building and working on
- **[Blog](/blog)** — Notes on construction tech, tools, and what I'm learning
- **[About](/about)** — More about me and what I do

---

## Latest Posts

{% for post in site.posts limit:5 %}
- **[{{ post.title }}]({{ post.url | relative_url }})** — {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
