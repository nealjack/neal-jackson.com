---
layout: page
years: [2015, 2016, 2017, 2018, 2019, 2020, 2022]
title: Publications
---


<div class="mdl-cell--8-col" markdown="1">
### Publications
{% for y in page.years reversed %}
  <h4  id="{{y}}" class="pubyear">{{y}}</h4>
  {% bibliography -f references -q @*[year={{y}}]* %}
{% endfor %}
</div>

