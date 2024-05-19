---
layout: post
title: "Russia Telegram Analysis - 2024-05-19"
author: "Dmytro Bukhanevych"
categories: analysis
tags: [telegram, analysis]
image: pawel-czerwinski-4x3VAM19wDA-unsplash.jpg
permalink: "/analysis/russia-telegram-analysis-2024-05-19"
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
<p>Загалом було проаналізовано 1605 постів у Telegram за 18.05.2024. Було відстежено активність 28 найбільш популярних Telegram каналів у Росії. Після попередньої обробки, фільтрування за ключовими словами, кластеризації та зменшення шуму, 185 текстів було проаналізовано у крайньому звітному періоді.</p>
<!-- Embedding Main Plotly Visualization -->
<div class="wide-iframe-container">
    <iframe src="{{site.baseurl}}/visualizations/2024-05-19/fig_topics_time.html" height="850"></iframe>
</div>


<h2>Cluster Text</h2>

<!-- Dropdown to select a cluster -->
<select id="clusterSelector" onchange="displayClusterText()">

</select>

<!-- Display area for the selected cluster's text -->
<div id="clusterTextDisplay" class="hidden"></div>

<script type="text/javascript">
    var clusterDetails = {};

    function displayClusterText() {
        var selectedLabel = document.getElementById("clusterSelector").value;
        var details = clusterDetails[selectedLabel];
        var textDiv = document.getElementById("clusterTextDisplay");
        textDiv.innerHTML = '<p>' + details + '</p>';
        textDiv.classList.remove('hidden');
    }
</script>

