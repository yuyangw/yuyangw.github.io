---
layout: page
permalink: /publications/
title: Publications
# description: 
years: [2023,2022,2021,2020]
nav: true
order: 2
---

<div class="publications">

My full list of publications can be found on <a href="https://scholar.google.com/citations?user=6eWGKEsAAAAJ&hl=en">Google Scholar</a> page.

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
