---
layout: default
title: Services
lang: en
---

# Services

<div style="background: linear-gradient(white, #f9d976); border: 1px solid black; padding: 1.5em; text-align: center; font-size: 20px; font-family: 'Arial', sans-serif; margin: 0 0 1em 0; width: calc(100% - 2em); max-width: 660px; height: 180px; display: flex; align-items: center; justify-content: center;">
  <span style="width:100%;">
    * <a href="/en/services/oem/01/" style="color: inherit; text-decoration: underline;">Cartridge OEM Manufacturing Service</a> *
  </span>
</div>

<div style="background: linear-gradient(white, #f9d976); border: 1px solid black; padding: 1.5em; text-align: center; font-size: 20px; font-family: 'Arial', sans-serif; margin: 0 0 1em 0; width: calc(100% - 2em); max-width: 660px; height: 180px; display: flex; align-items: center; justify-content: center;">
    * <a href="/en/services/repair.html" style="color: inherit; text-decoration: underline;">Cartridge Repair Service</a> *
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

![Cartridge 3](/assets/Cartridges/not-tappable-box.png)
