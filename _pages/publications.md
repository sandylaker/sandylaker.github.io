---
layout: page
permalink: /publications/
title: publications
description:  <span>&#42;</span> denotes equal contribution.
years: [2022, 2021, 2019]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
