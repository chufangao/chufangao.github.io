---
layout: page
permalink: /publications/
title: publications 
description: publications by categories in reversed chronological order. (* denotes equal contribution)
years: [2021, 2020, 2019, 2018]
submitted_years: [2022]
nav: true
---


<h3>Published works:</h3>

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>


