---
layout: page
permalink: /teaching/
title: Classes Taught
description:
nav: true
nav_order: 2
---

{% for class in site.data.teaching %}
  Semester: {{class.semester}} {{class.year}}
{% endfor %}

