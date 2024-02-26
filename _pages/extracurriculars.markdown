---
layout: single
permalink: /extracurriculars/
title: Extracurriculars
toc: true
toc_sticky: true

extracurriculars:
- title: Piano
  image_path: /assets/coffee.jpg
  excerpt: Every since first grade, I have been playing the piano. I love to play music and it has always been a part of me. Every year, I take the theory test and play in the Junior Festival and State Festival.
- title: Tennis
  image_path: /assets/coffee.jpg
  excerpt: My main sport is tennis. It is really fun and a balance between athleticism and technique. I have a lot of friends from tennis and I play tournaments whenever I can. Currently, I am planning to keep playing tennis outside of school, then play tennis in senior year of high school.
- title: FLL
  image_path: /assets/coffee.jpg
  excerpt: FLL is the lowest level of FIRST. I started FLL in seventh grade and programmed software. We programmed the robot using block coding, and I learned a lot about how the robot works. When we went to the competition, our robot got third place in the robot game. Unfortunately, our marketing was subpar, and we didn't move on.
- title: FTC
  image_path: /assets/coffee.jpg
  excerpt: FTC is the middle level of FIRST. I started FTC in eighth grade and programmed software, just like in FLL. FTC was based on the same principles, but went much more in depth with the programming. Instead of using block coding, we used Java and had to use the FTC Controller API to interact with the robot. I learned many things during FTC, such as PID Controllers, Velocity Controllers, Motion Planning, etc. At the competition, we got 11th place in our league. We were all happy with our season because we were a middle school team competing with high school teams with a lot more funding.
---

{% for ec in page.extracurriculars %}
## {{ ec.title }}
<div>{{ ec.excerpt }}</div>
{% endfor %}