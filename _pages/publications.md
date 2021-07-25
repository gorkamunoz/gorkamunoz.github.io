---
layout: page
permalink: /publications/
title: publications
description: Here is the full list of my publications. Reviewed articles are highlighted with the journal's abbreviation. Click the ABS button to deploy the abstract of each paper.
years: [2021,2020,2019,2017]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
