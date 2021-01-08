---
layout: page
permalink: /publications/
title: Publications
description: This page lists HTML links to my journal and conference papers, technical reports, dissertations, and theses.
years: [2020, 2018, 2017, 2016]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>