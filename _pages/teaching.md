---
layout: page
permalink: /teaching/
title: teaching
description: List of courses taught
nav: true
nav_order: 2
---

{% for entry in site.data.teaching %}

  ----
  <p><strong>{{entry.code}} {{entry.title}}</strong> {{entry.semester}} {{entry.year}} </p>
  <p>{{entry.institution}}. {{entry.level}} level.</p>
  {% if entry.cross %}
  Cross-listed as {{ entry.cross }}.
  {% endif %}
  
  _Catalog description_: {{entry.catalog_entry}}

  {% if entry.syllabus %}
  [Syllabus](/assets/pdf/{{entry.syllabus}})
  {% endif %}

  {% if entry.website %}
  [Website]({{entry.website}})
  {% endif %}

{% endfor %}
