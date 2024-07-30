---
layout: page
permalink: /teaching/
title: Teaching
description: List of courses taught
nav: true
nav_order: 2
---

{% for entry in site.data.teaching %}

  ----
  <p><strong>{{entry.code}} {{entry.title}}</strong> &emsp {{entry.semester}} {{entry.year}} </p>
  <p>{{entry.institution}}. {{entry.level}} level.</p>
  {% if entry.cross %}
      <p> Cross-listed as {{ entry.cross }}. </p>
  {% endif %}
  _Catalog description_: {{entry.catalog_entry}}
  
  
{% endfor %}

