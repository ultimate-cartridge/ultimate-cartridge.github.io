---
layout: default
title: Services
lang: en
---

# Services


<div class="service-box">
  <img src="/assets/services/bg-service-box.png" />
  <span style="width:100%;">
    <a href="/en/services/oem/01/" class="service-link">* Cartridge OEM Manufacturing Service *</a>
  </span>
</div>

<div class="service-box">
    <a href="/en/services/repair.html" class="service-link">* Cartridge Repair Service * </a> 
</div>

<!-- 自动列出 en/services/OEM 文件夹下的所有页面 -->
<ul>
  {% assign cartridge_pages = site.pages | where_exp: "page", "page.path contains 'en/services/OEM/'" %}
  {% for page in cartridge_pages %}
    {% if page.title and page.url != page.dir %}
      <li><a href="{{ page.url }}">{{ page.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

![Cartridge 3](/assets/products/not-tappable-box.png)
