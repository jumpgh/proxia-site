---
layout: products
title: Оборудование
permalink: /products/
description: Любые электро-, тепло-, водо-, газо- счетчики, имеющие импульсный выход – подключаются к системе мониторинга «Спрут-М» без дополнительных модулей!
---

<div class="products cardbox">
{%- for product in site.products -%}
<div class="card">
  <div class="optional-header">
    <div class="thumbnail thumbnail--40x40"><img src="https://image.flaticon.com/icons/png/512/1185/1185915.png" alt="" width="40" height="40"></div>
    <div class="primary-title">
      <div class="title">{{ product.model }}</div>
      <div class="subhead">{{ product.vendor }}</div>
    </div>
  </div>
  <div class="media media--16-9"> 
    <img src="https://media.pixeltuner.de/wp-content/uploads/2018/06/Shapes-Abstraction-Background-2466799.jpg" alt="" width="640" height="426"> 
  </div>
  <div class="primary-title">
    <div class="primary-text">{{ product.category }}</div>
    <div class="secondary-text">{{ product.usage }}</div>
  </div>
  <div class="supporting-text">{{ product.brief | truncate: 120, " .."}}</div>
    <div class="actions">
      <div class="action-buttons">
      	<a href="{{ product.url }}" class="button">details</a>
    </div>
    <div class="action-icons float-right"> <i class="material-icons action-icon" role="button" title="More options">more_vert</i> 
    </div>
  </div>
</div>
{%- endfor -%}
</div>