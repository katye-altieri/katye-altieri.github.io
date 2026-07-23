---
layout: archive
title: "Students"
permalink: /students/
author_profile: true
---

{% include base_path %}

{% for student in site.data.students %}
- **{{ student.name }}** ({{ student.degree }}, {{ student.year }})  
  Email: {{ student.email }}
{% endfor %}
