---
title: "local-job-scraper"
date: 2026-02-20
categories: projects
image: https://avatars.githubusercontent.com/u/189427369?s=400&u=8831cbc7eb1e73271f9de0aa1beb83ca0e930030&v=4
---

built a python tool this week that scrapes company websites directly for job openings — not indeed, not ziprecruiter.

the problem it solves: a lot of small and mid-size companies — especially contractors, suppliers, and service businesses — post jobs exclusively on their own websites. they never make it to the boards. you'd never find them unless you happened to land on the right `/careers` page at the right time.

the tool searches google maps for companies matching whatever industry types you configure, pulls their websites, checks for a careers page, and scans it for job titles you're looking for. it runs automatically every monday via github actions so you always have a fresh list.

three output buckets:
- **keyword matches** — career page found, your target title is listed
- **has a careers page** — worth bookmarking and checking back
- **no careers page** — worth a cold call or walk-in

everything is configurable in a single `config.py` file — your location, search radius, company types, and job keywords. no touching the core script.

built with python, beautifulsoup, and the google places api (new). runs free on github actions.

→ [github.com/ContractorKeith/local-job-scraper](https://github.com/ContractorKeith/local-job-scraper)