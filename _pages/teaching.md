---
layout: page
permalink: /teaching/
title: Classes Taught
description:
nav: true
nav_order: 2
---

{% for entry in site.data.teaching %}
  {{entry.title}}
  {{entry.semester}}, {{entry.year}}
  
{% endfor %}

