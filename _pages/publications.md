---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
types: [Journal, Conference/Workshop]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

<div class="publications">

{%- for t in page.types %}
  <h2 class="type">{{t}}</h2>
  {% bibliography -f papers -q @*[type={{t}}]* %}
{% endfor %}

</div>
