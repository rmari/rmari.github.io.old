---
layout: page
permalink: /collaborators/
title: collaborators
description: 
---

{% assign sorted_coauthors = site.data.coauthors | sort %}

<!-- <div class="profile col one right"> -->
<ul>
	{% for collab in sorted_coauthors %}
	<li>
	  {% if collab[1].url != null %}
		  <a href="{{collab[1].url}}">{{collab[1].firstname}} {{collab[0]}}</a>
	  {% else %}
		  {{collab[1].firstname}} {{collab[0]}}
	  {% endif %}
	</li>
	{% endfor %}
</ul>
<!-- </div> -->
