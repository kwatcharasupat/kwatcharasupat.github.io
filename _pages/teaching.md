---
layout: page
permalink: /teaching/
title: teaching
description:
nav: true
nav_order: 6
---
{% for course in site.teaching %}
  <h2><a href="{{ course.url }}">{{ course.course_code }}: {{ course.title }}</a></h2>
  <p>{{ course.semester }} at {{ course.university }} ({{ course.role }})</p>
  <p>{{ course.description }}</p>
{% endfor %}

<h1>guest lectures</h1>


{% for lecture in site.guest_lectures %}
  <h2><a href="{{ lecture.url }}">{{ lecture.course_code }}: {{ lecture.course_title }}</a></h2>
  <h3>{{ lecture.title }}</h3>
  <p>{{ lecture.semester }} at {{ lecture.university }}</p>
  <p>{{ lecture.description }}</p>
{% endfor %}