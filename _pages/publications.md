---
layout: page
permalink: /publications/
title: Publications
description: My publications are gathered below and can be found on my [Google Scholar webpage](https://scholar.google.com/citations?hl=fr&user=zKw3-kgAAAAJ).
years: [2023]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
