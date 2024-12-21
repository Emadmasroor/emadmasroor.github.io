---
layout: page
permalink: /teaching/
title: Teaching
description: 
years_instructor: [2023-24,2024-25]]
years_lecturer: [2024/25,2023/24,2022/23,2020/21,2019/20]
years_tutor: [2017/18,2016/17,2015/16,2014/15,2012/13]
nav: true
nav_order: 6
---


<p> 
All the courses I taught as 
</p>

<p>
<ul>
    <li><a href="#lecturer"><b>Lecturer</b></a></li>
    <li><a href="#tutor"><b>Teaching Assistant</b></a></li>
</ul>
</p>




<div class="publications">


<a id="lecturer"><h3 style="margin-top: 3.3rem; margin-bottom: -1.0rem;"><b>Lecturer</b></h3></a>

{%- for y in page.years_lecturer %}    
    <h2 class="year">{{ y }}</h2>
        {% bibliography -f teaching_lecturer -q @*[yearacademic={{y}}]* %}
{% endfor %}


<a id="instructor"><h3 style="margin-top: 3.3rem; margin-bottom: -1.0rem;"><b>Instructor</b></h3></a>
{%- for y in page.years_instructor %}    
    <h2 class="year">{{ y }}</h2>
        {% bibliography -f teaching_instructor -q @*[yearacademic={{y}}]* %}
{% endfor %}



<a id="tutor"><h3 style="margin-top: 5rem; margin-bottom: -1.0rem;"><b>Teaching Assistant</b></h3></a>

{%- for y in page.years_tutor %}    
    <h2 class="year">{{ y }}</h2>
        {% bibliography -f teaching_tutor -q @*[yearacademic={{y}}]* %}
{% endfor %}


</div>

