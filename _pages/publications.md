---
layout: page
permalink: /publications/
title: publications
description: publications in reverse chronological order.
years: [In preparation, 2021, 2017]
nav: true
---
 <!--_pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  <h2 class="year">"    "</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
