---
layout: page
title: Packages
excerpt: "R Packages"
modified: 2014-08-08T20:04:41.231140-04:00
#image:
#  feature: box-border.png
---

List of Swedish R packages:

<table style="width:100%">
  <tr>
    <th>Package</th>
    <th>Description</th> 
    <th>Links</th>
  </tr>
{% for package in site.data.packages %}
  <tr>
    <td>{{ package.name }}</td>
    <td>{{ package.description }}</td> 
    <td>
      {% if package.url contains 'http' %}<a class='fa fa-home' href='{{ package.url }}'></a>{% endif %}
      {% if package.github %}<a class='fa fa-github-square' href='https://github.com/{{ package.github }}'></a>{% endif %}
    </td>
{% endfor %}
</table>
