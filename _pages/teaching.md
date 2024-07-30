---
layout: page
permalink: /teaching/
title: Teaching
description: List of courses taught
nav: true
nav_order: 2
---

{% for entry in site.data.teaching %}
  {{entry.title}}
  {{entry.semester}}, {{entry.year}}
  
{% endfor %}

