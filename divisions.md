---
title: Divisions
layout: index
---

<div class="map">

<img src="/assets/map.jpg" width="250%" height="500px">

</div>

<div class="maptext">
<ul>
{% assign divisions_alphabetical = site.data.divisions | sort: "division" %}
{% for division in divisions_alphabetical %}
 <li><a href = "{{ division.weburl }}">{{ division.division }}</a></li>
 {% endfor %}
 </ul>

</div>