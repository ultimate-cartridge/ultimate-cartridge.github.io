---
layout: default
title: Services
lang: ja
---

# Services

<div class="service-box">
  <img src="/assets/services/bg-service-box.png" alt="" />
  <div>
    <a href="/ja/services/oem/01/" class="service-link">*カートリッジOEM製造サービス*</a>
  </div>
</div>

<div class="service-box">
  <a href="/ja/services/repair.html" class="service-link">*カートリッジ修理サービス*</a>
</div>

<!-- 自動で ja/services/OEM フォルダ内の全ページをリスト -->
<ul>
  {% assign cartridge_pages = site.pages | where_exp: "page", "page.path contains 'ja/services/OEM/'" %}
  {% for page in cartridge_pages %}
    {% if page.title and page.url != page.dir %}
      <li><a href="{{ page.url }}">{{ page.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>


![Cartridge 3](/assets/products/not-tappable-box.png)
