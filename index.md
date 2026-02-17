---
title: Home
permalink: /
---

# Welcome

I'm ContractorKeith - been in construction as an electrician, plumber, GC, home builder, estimator, PM, owner, and anythinbg else you can think of, for 37yrs. I have spent the last couple of years trying to learn code, and I have broken more than I ever did building buildings...

## What You'll Find Here

- **[projects](/projects)** — if I complete anything, this is where you will find it.
- **[notes](/blog)** — notes on tech, tools, ai and what I'm learning
- **[about](/about)** — more about me and what I do

---

## Latest Posts

{% for post in site.posts limit:5 %}
- **[{{ post.title }}]({{ post.url | relative_url }})** — {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
