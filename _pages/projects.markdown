---
layout: single
permalink: /projects/
title: Projects
date: 2024-01-03
---

{% for project in site.data.projects %}
## [{{ project.name }}](https://github.com/{{ site.author.github }}/{{ project.repository }})
<img src="{{ project.img }}" width=300 class="{% cycle 'align-left', 'align-right' %}">
<div class="projects-div">{{ project.description }}</div>
{% endfor %}