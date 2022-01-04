---
title: HOME
layout: HOME
---
<div id = "gallery">
  {% assign sorted_exhibits = site.exhibits %}
  {% for exhibit in sorted_exhibits %}
    {% assign licence_url = site.data.licences | find: "licence", exhibit.licence %}
    {% assign division = site.data.divisions | find: "division", exhibit.division %}
    <div class = "">
      <a href = "{{ exhibit.url | relative_url }}"><img src="{{ exhibit.image-url }}" width = 250></a>
      <p class = ""><a href = "{{exhibit.url | relative_url}}">{{ exhibit.title }}</a></p>
      <p><a href = "{{ division.weburl}}">{{ exhibit.division }}</a></p>
      <p class = "">{{ exhibit.time }}</p>
    </div>
{% endfor %}
 
</div>

<div class="foot-container">
                <div class="kcl-dept">
                    <img src="/assets/kcl.jpg" alt="kcl-logo">
                    <h3>Faculty of<br>Arts &amp; Humanities</h3>
                </div>
                <div class="kcl-addy">
                    <p>Department of Digital Humanities<br>Strand Building, Strand, London WC2R 2LS<br>United Kingdom</p>
                </div>
            </div>

