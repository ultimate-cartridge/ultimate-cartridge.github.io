---
layout: default
lang: ja
---

{% assign first_top = site.top | where: "order", 1 | where: "lang", page.lang | first %}
{% if first_top %}
  <meta http-equiv="refresh" content="0; url={{ first_top.url }}" />
{% endif %}