---
layout: page
permalink: /publications/
title: Publications & Talks
description: 
years_talk: [2024,2023,2022,2021,2019,2018]
years_papers: [2024,2022,2021,2020]
nav: true
nav_order: 4
---
<!-- _pages/publications.md -->

<p>
<ul>
 <li><a href="#journal"><b>Journal Articles</b></a></li>
 <li><a href="#talk"><b>Academic Talks</b></a></li>

<!-- 
<div class="large-badges" style="margin-top: 1.2rem;">
    <a href="https://scholar.google.com/citations?user={{ site.data.scholar.id }}">
        <img src="https://img.shields.io/badge/citations-{{ site.data.scholar.citations }}-000000?style=flat" 
        alt="{{ site.data.scholar.citations }} Google Scholar citations">
    </a>
    <a href="https://scholar.google.com/citations?user={{ site.data.scholar.id }}" aria-label="Google Scholar link" role="button">
        <img src="https://img.shields.io/badge/h--index-{{ site.data.scholar.h_index }}-000000?style=flat" 
        alt="{{ site.data.scholar.h_index }} Google Scholar h-index">
    </a>
    <a href="https://scholar.google.com/citations?user={{ site.data.scholar.id }}" aria-label="Google Scholar link" role="button">
        <img src="https://img.shields.io/badge/i10--index-{{ site.data.scholar.i10_index }}-000000?style=flat" 
        alt="{{ site.data.scholar.i10_index }} Google Scholar i10-index">
    </a>
</div>
-->



<div class="publications">

<a id="journal"><h3 style="margin-top: 3rem; margin-bottom: 0.3rem;"><b>Articles</b></h3></a>
<hr style="color: var(--global-text-color); height: 1px; margin-bottom: 2rem;">
{% bibliography -f papers %}

<a id="talk"><h3 style="margin-top: 5rem; margin-bottom: -1.0rem;"><b>Talks</b></h3></a>

{%- for y in page.years_talk %}
    <h2 class="year">{{ y }}</h2>
        {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}

</div>


