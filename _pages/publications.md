---
layout: page
permalink: /publications/
title: publications
description: 
years: [2021,2020,2019,2018,2017,2016,2014,2013]
nav: true
---

<div class="publications">

<h3>Journal articles</h3>
<h6>Please, reach out if you don't have access to the papers below.</h6>

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<!-- <h3>grey literature</h3>

{% bibliography -q @phdthesis @ %}

</div> -->
