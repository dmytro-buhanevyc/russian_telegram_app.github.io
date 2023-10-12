---
layout: post
title: "Russia Telegram Analysis - 2023-10-12"
author: "Dmytro Bukhanevych"
categories: analysis
tags: [telegram, analysis]
image: pawel-czerwinski-arwTpnIUHdM-unsplash.jpg
permalink: "/analysis/russia-telegram-analysis-2023-10-12"
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
<p>A total of 9483 Telegram posts were analyzed over the span of October 10, 2023 to October 11, 2023. The activity of 107 most-subscribed Telegram channels in Russia was monitored. Following a process of text preprocessing, keyword filtering, clustering, and noise reduction, 1360 posts were analyzed in the final reporting period.</p>
<!-- Embedding Main Plotly Visualization -->
<div class="wide-iframe-container">
    <iframe src="{{site.baseurl}}/visualizations/2023-10-12/fig_topics_time.html" height="850"></iframe>
</div>
<h2>Cluster Text</h2>
<p>Select a cluster to view the most representative post of the topic. Details on how the 'central' post is selected can be viewed in Methodology</p>
<!-- Dropdown to select a cluster -->
<select id="clusterSelector" onchange="displayClusterText()">

</select>
<!-- Button to toggle the display -->
<button onclick="displayClusterText()">Display Cluster Text</button>
<!-- Display area for the selected cluster's text -->
<div id="clusterTextDisplay" class="hidden"></div>
...
<script type="text/javascript">
    var clusterDetails = JSON.parse('{}');
    function displayClusterText() {
        ...
    }
</script>
