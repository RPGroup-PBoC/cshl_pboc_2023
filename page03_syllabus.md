---
layout: page
title: Syllabus
img: reading.png 
permalink: syllabus
caption: "DNA Sequence Chromatogram"
sidebar: true
---

<table>
<tr>
    <th><b>Date</b></th>
    <th><b>Topics</b></th>
    <th><b>Slides</b></th>
    <!-- <th><b>Reading</b></th> -->
</tr>
{% for day in site.data.syllabus %}
<tr>
    <td>{{day.date}}</td>
    <td>{{day.topic}}</td> 
    {% if day.slides %}
    <td><a href="{{site.data_url}}/{{day.slides}}">
    PDF </a></td>
    {% else %}
    <td>  </td>
    {% endif %}
    <!-- <td>{{day.reading}}</td> -->
</tr>
{% endfor %}
</table>