---
layout: page
permalink: /publications/
title: publications
description: See full list on <a href="https://scholar.google.com/citations?user=2hYADO4AAAAJ&hl=en">Google Scholar</a>.
years: [2021, 2019, 2018, 2017, 2016]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
