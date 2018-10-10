---
layout: page
permalink: /publications/
title: publications
description: 
---



{% for y in (2009..2018) reversed %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
