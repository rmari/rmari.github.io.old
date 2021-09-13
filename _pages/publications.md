---
layout: page
permalink: /publications/
title: publications
description: 
years: [2009, 2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021]
nav: true
---

<div class="publications">

{% for y in page.years reversed%}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
