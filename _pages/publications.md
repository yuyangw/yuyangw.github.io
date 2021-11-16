---
layout: page
permalink: /publications/
title: Publications
# description: 
years: [2021,2020]
nav: true
order: 2
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
