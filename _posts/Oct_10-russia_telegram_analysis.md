---
layout: post
title: "Russia Telegram Analysis - Oct_10"
author: "Dmytro Bukhanevych"
categories: analysis
tags: [telegram, analysis]
image: pattern.jpg
---
<style>
    /* Adjusting iframe-container styles */
    .wide-iframe-container {
        width: calc(100% + 30vw);  /* Extending the width */
        margin-left: -15vw;       /* Negative margin to push to the left */
        overflow: hidden;         /* In case the iframe content spills over */
    }
    .wide-iframe-container iframe {
        width: 100%;  /* Making the iframe take the full width of its container */
        border: none; /* Removing any borders from the iframe */
    }
    /* Toggle mechanism */
    .hidden {
        display: none;
    }
    .show-content-target:checked + .show-content {
        display: block;
    }
</style>
<h2>Main Topics</h2>
<p>A total of 9904 Telegram posts were analyzed during the period from October 09, 2023 to October 10, 2023. 102 most subscribed Telegram channels in Russia were monitored. During this reporting period 2959 posts matched our keywords.</p>
<!-- Embedding Main Plotly Visualization -->
<div class="wide-iframe-container">
    <iframe src="{{site.baseurl}}/visualizations/Oct_10/fig_topics_time.html" height="800"></iframe>
</div>
<!-- Toggle mechanism for the second graph: Line Total -->
<input type="checkbox" class="hidden show-content-target" id="showLineTotal">
<label for="showLineTotal">Click to show/hide Line Total</label>
<div class="show-content hidden wide-iframe-container">
    <iframe src="{{site.baseurl}}/visualizations/Oct_10/fig_line_total.png" height="800"></iframe>
</div>
<!-- Toggle mechanism for the third graph: Heatmap -->
<input type="checkbox" class="hidden show-content-target" id="showHeatmap">
<label for="showHeatmap">Click to show/hide Heatmap</label>
<div class="show-content hidden wide-iframe-container">
    <iframe src="{{site.baseurl}}/visualizations/Oct_10/fig_heatmap.png" height="800"></iframe>
</div>
<!-- Toggle mechanism for the fourth graph: Pie Chart -->
<input type="checkbox" class="hidden show-content-target" id="showPie">
<label for="showPie">Click to show/hide Pie Chart</label>
<div class="show-content hidden wide-iframe-container">
    <iframe src="{{site.baseurl}}/visualizations/Oct_10/fig_pie.png" height="800"></iframe>
</div>
