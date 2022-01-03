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
 <div id = "footer">
            <p>Creat by Chenkai, Zhuoqun, Mengxin, Ruowei</p>
  </div>
