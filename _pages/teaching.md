---
layout: page
permalink: /teaching/
title: Teaching
description: 
years_instructor: [2023-24,2024-25]
nav: true
nav_order: 6
---


<p> 
All the courses I taught as 
</p>

<p>
<ul>
    <li><a href="#instructor"><b>Instructor</b></a></li>
    <li><a href="#tutor"><b>Teaching Assistant</b></a></li>
</ul>
</p>




<div class="publications">


<a id="instructor"><h3 style="margin-top: 3.3rem; margin-bottom: -1.0rem;"><b>Visiting Assistant Professor at Swarthmore</b></h3></a>
{%- for y in page.years_instructor %}    
    <h2 class="year">{{ y }}</h2>
        {% bibliography -f teaching_instructor -q @*[yearacademic={{y}}]* %}
{% endfor %}



<a id="tutor"><h3 style="margin-top: 5rem; margin-bottom: -1.0rem;"><b>Teaching Assistant</b></h3></a>

</div>

