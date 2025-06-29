---
layout: default
lang: en
---

{% assign first_news = site.news | where: "lang", page.lang | sort: "date" | last %}
{% if first_news %}
  <meta http-equiv="refresh" content="0; url={{ first_news.url }}" />
{% endif %}