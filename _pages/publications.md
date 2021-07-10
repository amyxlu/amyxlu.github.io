---
layout: page
permalink: /publications/
title: publications
description: Conference and workshop papers exploring machine learning and computational biology.
years: [2021, 2020, 2019, 2018]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}