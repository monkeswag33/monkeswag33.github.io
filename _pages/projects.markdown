---
layout: single
permalink: /projects/
title: Projects
toc: true
toc_sticky: true

projects:
- name: PivotOS
  img: /assets/coffee.jpg
  repository: pivot-os
  description: >
    PivotOS, my custom operating system, started its journey in April 2023. After going to multiple iterations and multiple programming languages, I finally settled on Assembly and C. It has many features, such as a memory manager, multitasking and multiprocessing. It has taught me a lot about low level programming, memory, and debugging. As of right now, I am still interested in implementing more features in my operating system.
- name: Archive Tool
  img: /assets/coffee.jpg
  repository: archive-tool
  description: >
    I started this project in October 2022. While learning about compression algorithms and CMake, I decided to create a tool like tar, that would take in a directory and compress it to a file. It is written in C and while it is a small project, it taught me a lot about compression and archiving tools.
- name: Compressor
  img: /assets/coffee.jpg
  repository: compressor-zig
  description: >
    While learning about Zig and Huffman Coding, I wanted to experiment with it. Huffman Coding works by representing each byte as a combination of bits, so if a file uses the same characters multiple times, they can be represented by less than 8 bits. Through this project, I learned a lot about compression algorithms.
- name: Healthy Choices
  img: /assets/coffee.jpg
  repository: healthy-choices
  description: >
    When I found out about the Congressional App Challenge, I wanted to try it and see how I did. Because diabetes runs through my family, I wanted to make an app that handled the work that my parents did to decide what foods to eat. As a result, I ended up with an app called Healthy Choices that calculates the number of carbohydrates for all different types of food.
- name: Face Gender/Age Predictor
  img: /assets/coffee.jpg
  repository: age-prediction
  description: >
    While learning about machine learning, I created a project to predict the age and gender from a face. It uses the UTKFace dataset, which contains faces with all the information about them. This project had an accuracy of ~80%.
---

{% for project in page.projects %}
## [{{ project.name }}](https://github.com/{{ site.author.github }}/{{ project.repository }})
<!-- <img src="{{ project.img }}" width=300 class="{% cycle 'align-left', 'align-right' %}"> -->
<div class="projects-div">{{ project.description }}</div>
{% endfor %}