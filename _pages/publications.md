---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
types: [Journal, Conference]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->

<div class="publications">

{%- for t in page.types %}
  <h2 class="type" data-toggle="collapse" href="#{{t}}" aria-expanded="true" aria-controls={{t}}>
    {{t}}
  </h2>
  <div class="collapse show" id={{t}}>  
    {% bibliography -f papers -q @*[type={{t}}]* %}
  </div>
{% endfor %}

</div>
