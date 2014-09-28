---
layout: page
title: About
excerpt: "..."
modified: 2014-08-08T19:44:38.564948-04:00
image:
  feature: #so-simple-sample-image-4.jpg
  credit: #WeGraphics
  creditlink: #http://wegraphics.net/downloads/free-ultimate-blurred-background-pack/
---

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## Stockholm R User Group

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.

### Contributors

{% for i in site.data.authors %}
{% assign author = i[1] %}
<ul style="list-style-type:none">
<li style="float:left;margin:20px">
<center>
{% if author.avatar contains 'http' %}
<img src="{{ author.avatar }}" class="bio-photo" alt="{{ author.name }} bio photo"></a>
{% else %}
<img src="{{ site.url }}/images/{{ author.avatar }}" class="bio-photo" alt="{{ author.name }} bio photo"></a>
{% endif %}
{{ author.name }}<br>
{% if author.groups contains 'srug' %}<i>Steering Committee</i>{% endif %}<br>
{% if author.email %}<a class='fa fa-envelope' href="mailto:{{ author.email }}" target="_top"></a>&nbsp;{% endif %}
{% if author.linkedin %}<a class='fa fa-linkedin' href='https://www.linkedin.com/in/{{ author.linkedin }}'></a>&nbsp;{% endif %}
{% if author.github %}<a class='fa fa-github-square' href='https://github.com/{{ author.github }}'></a>&nbsp;{% endif %}<br>
</center>
</li>
</ul>

{% endfor %}
<div style="clear:both;"></div>

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
