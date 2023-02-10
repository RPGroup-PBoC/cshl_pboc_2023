---
layout: page
title: Code
img: code.png # Add image post (optional)
permalink: code
sidebar: true
---

---

During this course, you will develop a computational prowess that will aid in
your understanding of physical biology.  These will
be done using Jupyter notebooks through [Google
Colab](https://colab.research.google.com/), so you will need to sign into a
Google Account to create new notebooks. If you would like to set up Python on
your own computers, follow Tutorial 0a below. As the course progresses, we will
post the discussed or related notebooks below.

 We will post links to Jupyter Notebooks hosted on colab of the tutorial
sessions here. 


{% for topic in site.data.code %}
# {{topic[0]}}
{% for script in topic[1] %}

* [**{{script.title}}**]({{script.colab}}) \|
  {{script.description}}  {%if script.links %} <i>{%for l in script.links
  %}[**\[{{l[0]}}\]**](assets/code/{{l[1]}}){%endfor%}</i>{%endif%}
{% endfor %}
{%endfor%}