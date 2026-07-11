---
layout: page
title: Solar Time
description: A solar clock for any location
img: assets/img/solarclock.png
importance: 1
category: fun
---

<div class="streamlit-container">
    <iframe 
        src="https://solar-time.streamlit.app/?embed=true"
        width="100%" 
        height="850px" 
        style="border: none; border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.08);"
        allow="geolocation">
    </iframe>
</div>

<style>
    /* This makes sure the app spans cleanly on small mobile viewports */
    .streamlit-container {
        width: 100%;
        margin-top: 20px;
        margin-bottom: 40px;
    }
</style>
