---
layout: page
permalink: /publications/
title: publications
#description: \* denotes equal contribution
years: [2025, 2024, 2023, 2022, 2020, 2019, 2018, 2017, 2016] # 2021, 2015
nav: true
---

\* denotes equal contribution

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
