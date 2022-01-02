---
title: Gallery index
layout: index
---

{% for exhibit in site.exhibits %}

<img src="{{ exhibit.image-url }}" width = 250>
<p>{{ exhibit.title }} in {{ exhibit.division}}</p>
<p><a href="{{ exhibit.licence-url }}">{{ exhibit.licence }}</a></p>

{% endfor %}