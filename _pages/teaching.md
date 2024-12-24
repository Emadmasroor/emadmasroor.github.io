---
layout: page
permalink: /teaching/
title: Teaching
description: 
years_instructor: [2024-25,2023-24]
years_vt: [2021-22]
nav: true
nav_order: 6
---


<p> 
All the courses I taught as 
</p>

<p>
<ul>
    <li><a href="#VAP"><b>Visiting Assistant Professor</b></a></li>
    <li><a href="#ior"><b>Instructor of Record</b></a></li>
</ul>
</p>




<div class="publications">


<a id="VAP"><h3 style="margin-top: 3.3rem; margin-bottom: -1.0rem;"><b>Visiting Assistant Professor at Swarthmore</b></h3></a>
{%- for y in page.years_instructor %}    
    <h2 class="year">{{ y }}</h2>
        {% bibliography -f teaching_vap -q @*[yearacademic={{y}}]* %}
{% endfor %}


<a id="ior"><h3 style="margin-top: 3.3rem; margin-bottom: -1.0rem;"><b>Instructor of Record at Virginia Tech</b></h3></a>
{%- for y in page.years_vt %}    
    <h2 class="year">{{ y }}</h2>
        {% bibliography -f teaching_vt -q @*[yearacademic={{y}}]* %}
{% endfor %}


</div>

