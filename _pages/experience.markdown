---
layout: single
title: Volunteering
permalink: /volunteering/
toc: true
toc_sticky: true

experience:
  - title: FTC Stem Night
    image_path: /assets/coffee.jpg
    excerpt: >
      While working in FTC, we went to teach the elementary school about STEM and robotics. We brought STEM kits that we helped them build and let them control our robot. We all learned a lot and had a fun time teaching them about STEM.
  - title: Library Volunteering
    image_path: /assets/coffee.jpg
    excerpt: >
      Over the summer, I went to the Lake Travis Library to volunteer. There, I helped parents and kids, shelved books, and put books in the vans. I had a really fun time and made a lot of friends, and I hope to return back next summer.
  - title: Tennis Volunteering
    image_path: /assets/coffee.jpg
    excerpt: Alongside the library volunteering, I helped volunteer at my former tennis coach's tennis summer camp. We had to stay out for 4 - 5 hours in the 90+ degrees heat, but a lot of my friends helped there and it was fun seeing the little kids learn. The summer camp was one of the most fun things I did during the summer.
---

{% for project in page.experience %}
## {{ project.title }}
<div class="experience-div">{{ project.excerpt }}</div>
{% endfor %}
