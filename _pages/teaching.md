---
layout: page
permalink: /teaching/
title: Teaching
description: List of courses taught
nav: true
nav_order: 2
---

{% for entry in site.data.teaching %}
  
  ** {{entry.code}}: {{entry.title}} at {{entry.institution}}**
  Term: {{entry.semester}} {{entry.year}}
  Level: {{entry.level}}
  
  
{% endfor %}

