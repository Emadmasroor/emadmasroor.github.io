---
layout: page
permalink: /teaching/
title: List of Classes
description: Course Materials
nav: true
nav_order: 2
---

{% for class in site.data.teaching %}
  {% class.semester %}
{% endfor %}

