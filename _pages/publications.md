---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2021]
nav: true
---
<div class="publications">

{%- for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
