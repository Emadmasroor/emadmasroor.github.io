---
layout: page
permalink: /presentations/
title: Presentations
description: 
years_talk: [2024,2023,2022,2021,2019,2018]
years_poster: [2021,2016]
years_institutional: [2024]
nav: true
nav_order: 6
---


<p> 
All my dissemination activity divided in 
</p>

<p> 
<ul>
    <li><a href="#talk"><b>Academic Talks</b></a></li>
    <li><a href="#poster"><b>Poster Presentations</b></a></li>
    <li><a href="#institutional"><b>Institutional Presentations</b></a></li>
</ul>
</p>


<p>
<i class="far fa-envelope" style="font-size: 0.85em;"></i> &nbsp; denotes invited contribution
</p>



<div class="publications">

<a id="talk"><h3 style="margin-top: 3.3rem; margin-bottom: -1.0rem;"><b>Academic Talks</b></h3></a>

{%- for y in page.years_talk %}    
    <h2 class="year">{{ y }}</h2>
        {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}



<a id="poster"><h3 style="margin-top: 5rem; margin-bottom: -1.0rem;"><b>Poster Presentations</b></h3></a>

{%- for y in page.years_poster %}    
    <h2 class="year">{{ y }}</h2>
        {% bibliography -f seminars_posters -q @*[year={{y}}]* %}
{% endfor %}



<a id="institutional"><h3 style="margin-top: 3.3rem; margin-bottom: -1.0rem;"><b>Institutional Presentations</b></h3></a>

{%- for y in page.years_institutional %}    
    <h2 class="year">{{ y }}</h2>
        {% bibliography -f seminars_institutional -q @*[year={{y}}]* %}
{% endfor %}


</div>
