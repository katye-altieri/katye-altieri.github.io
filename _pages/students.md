---
layout: archive
title: "Students"
permalink: /students/
author_profile: true
---

{% include base_path %}

## Current Students
{% for student in site.data.students %}
{% if student.status == "Current" %}
- **{{ student.name }}** ({{ student.degree }}, {{ student.year }})  
  Email: {{ student.email }}
{% endif %}
{% endfor %}

## Alumni
{% for student in site.data.students %}
{% if student.status == "Alumni" %}
- **{{ student.name }}** ({{ student.degree }}, {{ student.year }})
{% endif %}
{% endfor %}
