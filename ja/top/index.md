---
layout: default
title: Top
lang: ja
---


{% assign first_top = site.top | where: "lang", page.lang | sort: "date" | last %}
{% if first_top %}
  <meta http-equiv="refresh" content="0; url={{ first_top.url }}" />
{% endif %}