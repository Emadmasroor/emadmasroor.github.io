---
layout: page
title: Solar Time
description: A solar clock for any location
img: assets/img/solarclock.png
importance: 1
category: fun
---

View this on a standalone page at [solar-time.streamlit.app](https://solar-time.streamlit.app)

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
    /* Forces the iframe container to break out of the template's standard text margins */
    .streamlit-breakout {
        width: 100vw;
        position: relative;
        left: 50%;
        right: 50%;
        margin-left: -50vw;
        margin-right: -50vw;
        padding-left: 40px;  /* Adds clean gutter padding so it doesn't touch the viewport edge */
        padding-right: 40px;
    }
    
    @media (max-width: 768px) {
        .streamlit-breakout {
            padding-left: 15px;
            padding-right: 15px;
        }
    }
</style>
