---
layout: page
permalink: /teaching/
title: Teaching
description: List of courses taught
nav: true
nav_order: 2
---

{% for entry in site.data.teaching %}

  <p><strong>{{entry.code}} {{entry.title}}</strong></p>
  <p>{{entry.institution}}, {{entry.semester}} {{entry.year}}</p>
  <p> Catalog description: {{entry.catalog_entry}}</p>
  
  
{% endfor %}

