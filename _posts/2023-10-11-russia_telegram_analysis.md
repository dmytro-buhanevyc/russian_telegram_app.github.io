---
layout: post
title: "Russia Telegram Analysis - 2023-10-11"
author: "Dmytro Bukhanevych"
categories: analysis
tags: [telegram, analysis]
image: daniel-olah-VS_kFx4yF5g-unsplash.jpg
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
    <iframe src="{{site.baseurl}}/visualizations/2023-10-11/fig_topics_time.html" height="800"></iframe>
</div>
<h2>Cluster Posts Examples</h2><select id="clusterDropdown" onchange="displayClusterText()"><option value="0">Cluster 0</option><option value="1">Cluster 1</option><option value="2">Cluster 2</option><option value="3">Cluster 3</option><option value="4">Cluster 4</option><option value="5">Cluster 5</option><option value="6">Cluster 6</option><option value="7">Cluster 7</option><option value="8">Cluster 8</option><option value="9">Cluster 9</option><option value="10">Cluster 10</option><option value="11">Cluster 11</option><option value="12">Cluster 12</option></select><div id="displayedClusterText">Select a cluster from the dropdown to view its content.</div>
