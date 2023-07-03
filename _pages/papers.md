---
layout: page
permalink: /publications/
title: publications
description: Publications in reverse chronological order.
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2013, 2012, 2008]
nav: true
order: 20
---

<div class="publications">

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
