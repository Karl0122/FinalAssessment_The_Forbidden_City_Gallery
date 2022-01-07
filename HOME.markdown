---
title: HOME
layout: HOME
---
{% assign sorted_exhibits = site.exhibits %}
<!-- line one -->
<div class="main_box">
	<div class="line_title">
		<span>the Three Halls of Outer Court</span>
	</div>
	<div id = "gallery_line" class="gallery_line">
	{% for exhibit in sorted_exhibits %}
		{% assign licence_url = site.data.licences | find: "licence", exhibit.licence %}
		{% assign division = site.data.divisions | find: "division", exhibit.division %}
		{% if exhibit.lineType == 'lineTwo' %}
			<div class = "line_box">
			  <a href = "{{ exhibit.url | relative_url }}"><img src="{{ exhibit.image-url }}" width = 360 height = 270></a>
			  <p title="{{ exhibit.title }}" class = "line_img_box"><a href = "{{exhibit.url | relative_url}}">
				<span class="exhibit_title ">{{ exhibit.title }}</span>
				<br>
				<span >{{ exhibit.time }}</span>
			  </a></p>			  
			</div>
		{% endif %}
	{% endfor %}
	</div>
</div>
<!-- line two -->
<div class="main_box">
	<div class="line_title">
		<span>the Three Back Palaces</span>
	</div>
	<div id = "gallery_line" class="gallery_line">
	{% for exhibit in sorted_exhibits %}
		{% assign licence_url = site.data.licences | find: "licence", exhibit.licence %}
		{% assign division = site.data.divisions | find: "division", exhibit.division %}
		{% if exhibit.lineType == 'lineOne' %}
			<div class = "line_box">
			  <a href = "{{ exhibit.url | relative_url }}"><img src="{{ exhibit.image-url }}" width = 360 height = 270></a>
			  <p title="{{ exhibit.title }}" class = "line_img_box"><a href = "{{exhibit.url | relative_url}}">
				<span class="exhibit_title ">{{ exhibit.title }}</span>
				<br>
				<span >{{ exhibit.time }}</span>
			  </a></p>
			  
			</div>
		{% endif %}
	{% endfor %}
	</div>
</div>
<!-- line three -->
<div class="main_box">
	<div class="line_title">
		<span> the Six Western Palaces</span>
	</div>
	<div id = "gallery_line" class="gallery_line">
	{% for exhibit in sorted_exhibits %}
		{% assign licence_url = site.data.licences | find: "licence", exhibit.licence %}
		{% assign division = site.data.divisions | find: "division", exhibit.division %}
		{% if exhibit.lineType == 'lineThree' %}
			<div class = "line_box">
			  <a href = "{{ exhibit.url | relative_url }}"><img src="{{ exhibit.image-url }}" width = 360 height = 270></a>
			  <p title="{{ exhibit.title }}" class = "line_img_box"><a href = "{{exhibit.url | relative_url}}">
				<span class="exhibit_title ">{{ exhibit.title }}</span>
				<br>
				<span >{{ exhibit.time }}</span>
			  </a></p>
			</div>
		{% endif %}
	{% endfor %}
	</div>
</div>
<!-- line four -->
<div class="main_box">
	<div class="line_title">
		<span>the Six Eastern Palaces</span>
	</div>
	<div id = "gallery_line" class="gallery_line">
	{% for exhibit in sorted_exhibits %}
		{% assign licence_url = site.data.licences | find: "licence", exhibit.licence %}
		{% assign division = site.data.divisions | find: "division", exhibit.division %}
		{% if exhibit.lineType == 'lineFour' %}
			<div class = "line_box">
			  <a href = "{{ exhibit.url | relative_url }}"><img src="{{ exhibit.image-url }}" width = 360 height = 270></a>
			  <p title="{{ exhibit.title }}" class = "line_img_box"><a href = "{{exhibit.url | relative_url}}">
				<span class="exhibit_title ">{{ exhibit.title }}</span>
				<br>
				<span >{{ exhibit.time }}</span>
			  </a></p>
			</div>
		{% endif %}
	{% endfor %}
	</div>
</div>
<!-- line five -->
<div class="main_box">
	<div class="line_title">
		<span>Gates</span>
	</div>
	<div id = "gallery_line" class="gallery_line">
	{% for exhibit in sorted_exhibits %}
		{% assign licence_url = site.data.licences | find: "licence", exhibit.licence %}
		{% assign division = site.data.divisions | find: "division", exhibit.division %}
		{% if exhibit.lineType == 'lineFive' %}
			<div class = "line_box">
			  <a href = "{{ exhibit.url | relative_url }}"><img src="{{ exhibit.image-url }}" width = 360 height = 270></a>
			  <p title="{{ exhibit.title }}" class = "line_img_box"><a href = "{{exhibit.url | relative_url}}">
				<span class="exhibit_title ">{{ exhibit.title }}</span>
				<br>
				<span >{{ exhibit.time }}</span>
			  </a></p>
			</div>
		{% endif %}
	{% endfor %}
	</div>
</div>

<div id = "footer">
	<p>Creat by Chenkai, Zhuoqun, Mengxin, Ruowei</p>
</div>