---
order_id: 2
layout: page
permalink: /publications/
title: Publications
description: 
years: [2022, 2021]
nav: false
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
