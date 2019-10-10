---
layout: page
permalink: /publications/
title: publications
description: 
---



{% for y in (2009..2019) reversed %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
