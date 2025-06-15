---
layout: default
lang: ja
---

<!-- <meta http-equiv="refresh" content="0; url=/ja/Top/01/" /> -->
{% assign first_top = site.top | where: "order", 1 | first %}
{% if first_top %}
  <meta http-equiv="refresh" content="0; url={{ first_top.url }}" />
{% endif %}