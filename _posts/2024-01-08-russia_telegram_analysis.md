---
layout: post
title: "Russia Telegram Analysis - 2024-01-08"
author: "Dmytro Bukhanevych"
categories: analysis
tags: [telegram, analysis]
image: daniel-olah-KDCzAGuf0e8-unsplash.jpg
permalink: "/analysis/russia-telegram-analysis-2024-01-08"
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
<p>Загалом було проаналізовано 4465 постів у Telegram за 07.01.2024. Було відстежено активність 91 найбільш популярних Telegram каналів у Росії. Після попередньої обробки, фільтрування за ключовими словами, кластеризації та зменшення шуму, 579 текстів було проаналізовано у крайньому звітному періоді.</p>
<!-- Embedding Main Plotly Visualization -->
<div class="wide-iframe-container">
    <iframe src="{{site.baseurl}}/visualizations/2024-01-08/fig_topics_time.html" height="850"></iframe>
</div>


<h2>Cluster Text</h2>

<!-- Dropdown to select a cluster -->
<select id="clusterSelector" onchange="displayClusterText()">
<option value="0">Cluster 0</option><option value="1">Cluster 1</option><option value="2">Cluster 2</option><option value="3">Cluster 3</option><option value="4">Cluster 4</option><option value="5">Cluster 5</option><option value="6">Cluster 6</option><option value="7">Cluster 7</option><option value="8">Cluster 8</option><option value="9">Cluster 9</option>
</select>

<!-- Display area for the selected cluster's text -->
<div id="clusterTextDisplay" class="hidden"></div>

<script type="text/javascript">
    var clusterDetails = {"0": "<b>Total Posts:</b> 25<br><b>Date:</b> 2024-01-07 06:22:23+00:00<br><b>Author:</b> meduzalive<br><b>Link:</b> https://t.me/s/meduzalive/97942<br><b>Subscribers:</b> 1155510<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u041f\u0443\u0442\u0438\u043d \u043d\u0430 \u0420\u043e\u0436\u0434\u0435\u0441\u0442\u0432\u043e \u0432\u0441\u0442\u0440\u0435\u0442\u0438\u043b\u0441\u044f \u0441 \u0440\u043e\u0434\u0441\u0442\u0432\u0435\u043d\u043d\u0438\u043a\u0430\u043c\u0438 \u043f\u043e\u0433\u0438\u0431\u0448\u0438\u0445 \u0443\u0447\u0430\u0441\u0442\u043d\u0438\u043a\u043e\u0432 \u0432\u0442\u043e\u0440\u0436\u0435\u043d\u0438\u044f \u0432 \u0423\u043a\u0440\u0430\u0438\u043d\u0443\u042d\u0442\u0430 \u0432\u0441\u0442\u0440\u0435\u0447\u0430 \u0432 \u041d\u043e\u0432\u043e-\u041e\u0433\u0430\u0440\u0435\u0432\u043e, \u043a\u0430\u043a \u0437\u0430\u044f\u0432\u0438\u043b \u043f\u0440\u0435\u0437\u0438\u0434\u0435\u043d\u0442 \u0420\u0424, \u0434\u043e\u043b\u0436\u043d\u0430 \u0441\u0442\u0430\u0442\u044c \u00ab\u0441\u0438\u0433\u043d\u0430\u043b\u043e\u043c\u00bb \u0434\u043b\u044f \u0440\u043e\u0441\u0441\u0438\u0439\u0441\u043a\u0438\u0445 \u0447\u0438\u043d\u043e\u0432\u043d\u0438\u043a\u043e\u0432 \u0432\u0441\u0435\u0445 \u0443\u0440\u043e\u0432\u043d\u0435\u0439 \u043e \u0442\u043e\u043c, \u0447\u0442\u043e \u043f\u0440\u043e\u0431\u043b\u0435\u043c\u0430\u043c \u0432\u043e\u0435\u043d\u043d\u044b\u0445 \u0438 \u0438\u0445 \u0440\u043e\u0434\u0441\u0442\u0432\u0435\u043d\u043d\u0438\u043a\u043e\u0432 \u043d\u0443\u0436\u043d\u043e \u0443\u0434\u0435\u043b\u044f\u0442\u044c \u0431\u043e\u043b\u044c\u0448\u0435 \u0432\u043d\u0438\u043c\u0430\u043d\u0438\u044f. \u00ab\u0425\u043e\u0447\u0443 \u0435\u0449\u0435 \u0440\u0430\u0437 \u0432\u0430\u0441 \u0437\u0430\u0432\u0435\u0440\u0438\u0442\u044c, \u0447\u0442\u043e \u043c\u044b \u0432\u0441\u0435\u0433\u0434\u0430 \u0431\u0443\u0434\u0435\u043c \u0440\u044f\u0434\u043e\u043c \u0441 \u0432\u0430\u043c\u0438\u00bb, \u2014 \u0441\u043a\u0430\u0437\u0430\u043b \u043e\u043d.\u041f\u043e\u0441\u043b\u0435 \u044d\u0442\u043e\u0433\u043e \u041f\u0443\u0442\u0438\u043d \u0438 \u0447\u043b\u0435\u043d\u044b \u0441\u0435\u043c\u0435\u0439 \u0443\u0447\u0430\u0441\u0442\u043d\u0438\u043a\u043e\u0432 \u0432\u043e\u0439\u043d\u044b \u043f\u043e\u0441\u0435\u0442\u0438\u043b\u0438 \u0441\u043b\u0443\u0436\u0431\u0443 \u0432 \u0446\u0435\u0440\u043a\u0432\u0438 \u0432 \u041d\u043e\u0432\u043e-\u041e\u0433\u0430\u0440\u0435\u0432\u043e. \u0420\u0430\u043d\u0435\u0435 \u0441\u043e\u043e\u0431\u0449\u0430\u043b\u043e\u0441\u044c, \u0447\u0442\u043e \u043f\u0440\u0435\u0437\u0438\u0434\u0435\u043d\u0442 \u0420\u0424 \u043c\u043e\u0436\u0435\u0442 \u043f\u0440\u0438\u0435\u0445\u0430\u0442\u044c \u0432 \u0425\u0440\u0430\u043c \u0425\u0440\u0438\u0441\u0442\u0430 \u0421\u043f\u0430\u0441\u0438\u0442\u0435\u043b\u044f, \u0433\u0434\u0435 \u0432\u044b\u0441\u0442\u0430\u0432\u0438\u043b\u0438 \u00ab\u0422\u0440\u043e\u0438\u0446\u0443\u00bb \u0410\u043d\u0434\u0440\u0435\u044f \u0420\u0443\u0431\u043b\u0435\u0432\u0430.\u0412 \u0441\u0432\u043e\u0435\u043c \u0440\u043e\u0436\u0434\u0435\u0441\u0442\u0432\u0435\u043d\u0441\u043a\u043e\u043c \u043e\u0431\u0440\u0430\u0449\u0435\u043d\u0438\u0438 \u041f\u0443\u0442\u0438\u043d \u0442\u0430\u043a\u0436\u0435 \u0437\u0430\u0442\u0440\u043e\u043d\u0443\u043b \u0442\u0435\u043c\u0443 \u0432\u043e\u0439\u043d\u044b \u0432 \u0423\u043a\u0440\u0430\u0438\u043d\u0435, \u043e\u0431\u0440\u0430\u0442\u0438\u043b\u043e \u0432\u043d\u0438\u043c\u0430\u043d\u0438\u0435 \u00ab\u0410\u0433\u0435\u043d\u0442\u0441\u0442\u0432\u043e\u00bb. \u00ab\u0413\u043b\u0443\u0431\u043e\u043a\u043e\u0433\u043e, \u0438\u0441\u043a\u0440\u0435\u043d\u043d\u0435\u0433\u043e \u0443\u0432\u0430\u0436\u0435\u043d\u0438\u044f \u0437\u0430\u0441\u043b\u0443\u0436\u0438\u0432\u0430\u044e\u0442 \u0443\u0441\u0438\u043b\u0438\u044f \u0440\u0435\u043b\u0438\u0433\u0438\u043e\u0437\u043d\u044b\u0445 \u043e\u0440\u0433\u0430\u043d\u0438\u0437\u0430\u0446\u0438\u0439, \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u043d\u044b\u0435 \u043d\u0430 \u043f\u043e\u0434\u0434\u0435\u0440\u0436\u043a\u0443 \u043d\u0430\u0448\u0438\u0445 \u0433\u0435\u0440\u043e\u0435\u0432 \u2014 \u0443\u0447\u0430\u0441\u0442\u043d\u0438\u043a\u043e\u0432 \u0441\u043f\u0435\u0446\u0438\u0430\u043b\u044c\u043d\u043e\u0439 \u0432\u043e\u0435\u043d\u043d\u043e\u0439 \u043e\u043f\u0435\u0440\u0430\u0446\u0438\u0438, \u0436\u0438\u0442\u0435\u043b\u0435\u0439 \u0414\u043e\u043d\u0431\u0430\u0441\u0441\u0430 \u0438 \u041d\u043e\u0432\u043e\u0440\u043e\u0441\u0441\u0438\u0438\u00bb, \u2014 \u0441\u043a\u0430\u0437\u0430\u043d\u043e \u043d\u0430 \u0441\u0430\u0439\u0442\u0435 \u041a\u0440\u0435\u043c\u043b\u044f.", "1": "<b>Total Posts:</b> 29<br><b>Date:</b> 2024-01-07 17:40:41+00:00<br><b>Author:</b> ukraina_ru<br><b>Link:</b> https://t.me/s/ukraina_ru/183589<br><b>Subscribers:</b> 355688<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \ud83c\uddf7\ud83c\uddfa \u0420\u0435\u0430\u043a\u0446\u0438\u044f \u041a\u0440\u0435\u043c\u043b\u044f \u043d\u0430 \u0432\u044b\u0441\u043a\u0430\u0437\u044b\u0432\u0430\u043d\u0438\u044f \u041a\u0443\u043b\u0435\u0431\u044b \u0431\u044b\u043b\u0430 \u043e\u0437\u0432\u0443\u0447\u0435\u043d\u0430 \u0437\u0430\u0434\u043e\u043b\u0433\u043e \u0434\u043e \u0432\u044b\u0441\u043a\u0430\u0437\u044b\u0432\u0430\u043d\u0438\u0439 \u041a\u0443\u043b\u0435\u0431\u044b\u041d\u043e \u0435\u0441\u043b\u0438 \u043d\u0443\u0436\u043d\u043e \u043f\u043e\u0432\u0442\u043e\u0440\u0438\u0442\u044c, \u0442\u043e \u0432\u043e\u0442 \u0441\u0432\u0435\u0436\u0435\u0435 \u0437\u0430\u044f\u0432\u043b\u0435\u043d\u0438\u0435 \u043f\u0435\u0440\u0432\u043e\u0433\u043e \u0437\u0430\u043c\u0435\u0441\u0442\u0438\u0442\u0435\u043b\u044f \u043f\u043e\u0441\u0442\u043e\u044f\u043d\u043d\u043e\u0433\u043e \u043f\u0440\u0435\u0434\u0441\u0442\u0430\u0432\u0438\u0442\u0435\u043b\u044f \u0420\u0424 \u043f\u0440\u0438 \u041e\u041e\u041d \u0414\u043c\u0438\u0442\u0440\u0438\u044f \u041f\u043e\u043b\u044f\u043d\u0441\u043a\u043e\u0433\u043e:\u0423\u043a\u0440\u0430\u0438\u043d\u0441\u043a\u0438\u0435 \u0432\u043e\u0439\u0441\u043a\u0430 \u0442\u043e\u0447\u043d\u043e \u043d\u0435 \u0441\u043e\u0431\u0438\u0440\u0430\u044e\u0442\u0441\u044f \u0438\u0434\u0442\u0438 \u043d\u0430 \u041c\u043e\u0441\u043a\u0432\u0443, \u043f\u043e\u0441\u043a\u043e\u043b\u044c\u043a\u0443 \u043a\u0438\u0435\u0432\u0441\u043a\u0438\u0439 \u0440\u0435\u0436\u0438\u043c \u0434\u043e\u0432\u043e\u043b\u044c\u043d\u043e \u0441\u043a\u043e\u0440\u043e \u043f\u0440\u043e\u0438\u0433\u0440\u0430\u0435\u0442. \u041d\u043e, \u043a\u0430\u043a \u043f\u043e\u043a\u0430\u0437\u044b\u0432\u0430\u0435\u0442 \u0443\u043a\u0440\u0430\u0438\u043d\u0441\u043a\u0438\u0439 \u043a\u0440\u0438\u0437\u0438\u0441, \u0441\u0443\u0449\u0435\u0441\u0442\u0432\u043e\u0432\u0430\u043d\u0438\u044e \u0420\u043e\u0441\u0441\u0438\u0438 \u0443\u0433\u0440\u043e\u0436\u0430\u0435\u0442 \u041d\u0410\u0422\u041e, \u043a\u043e\u0442\u043e\u0440\u0430\u044f \u0434\u0435-\u0444\u0430\u043a\u0442\u043e \u0432\u0435\u0434\u0451\u0442 \u0432\u043e\u0439\u043d\u0443 \u043d\u0430 \u0423\u043a\u0440\u0430\u0438\u043d\u0435 \u0447\u0435\u0440\u0435\u0437 \u0441\u0432\u043e\u0438\u0445 \u043f\u0440\u043e\u043a\u0441\u0438. \u042d\u0442\u043e \u0432\u0435\u0440\u0448\u0438\u043d\u0430 \u0434\u043e\u043b\u0433\u043e\u0441\u0440\u043e\u0447\u043d\u043e\u0439 \u0441\u0442\u0440\u0430\u0442\u0435\u0433\u0438\u0438 \u0421\u0428\u0410 \u043f\u043e \u043e\u0441\u043b\u0430\u0431\u043b\u0435\u043d\u0438\u044e, \u0430 \u0437\u0430\u0442\u0435\u043c \u0438 \u0440\u0430\u0437\u0433\u0440\u043e\u043c\u0443 \u0420\u043e\u0441\u0441\u0438\u0438.\u0414\u043c\u0438\u0442\u0440\u0438\u0439 \u041f\u043e\u043b\u044f\u043d\u0441\u043a\u0438\u0439, \u043e\u043f\u0443\u0431\u043b\u0438\u043a\u043e\u0432\u0430\u0432\u0448\u0438\u0439 \u044d\u0442\u0438 \u0441\u0442\u0440\u043e\u043a\u0438 \u0432 \u0441\u043e\u0446\u0441\u0435\u0442\u0438, \u043d\u0435 \u0441\u043e\u043c\u043d\u0435\u0432\u0430\u0435\u0442\u0441\u044f, \u0447\u0442\u043e \u043c\u0438\u0440 \u0438\u0437\u043c\u0435\u043d\u0438\u0442\u0441\u044f \u043f\u043e\u0441\u043b\u0435 \u043f\u043e\u0440\u0430\u0436\u0435\u043d\u0438\u044f \u041a\u0438\u0435\u0432\u0430 \u0438 \u0435\u0433\u043e \u0441\u0442\u043e\u0440\u043e\u043d\u043d\u0438\u043a\u043e\u0432.\u0417\u043d\u0430\u0442\u044c \u0431\u043e\u043b\u044c\u0448\u0435 \u0441 \u0423\u043a\u0440\u0430\u0438\u043d\u0430.\u0440\u0443", "2": "<b>Total Posts:</b> 20<br><b>Date:</b> 2024-01-07 10:45:01+00:00<br><b>Author:</b> readovkanews<br><b>Link:</b> https://t.me/s/readovkanews/72020<br><b>Subscribers:</b> 2303305<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u0411\u043e\u043b\u044c\u0448\u0430\u044f \u0432\u0435\u043b\u0438\u043a\u0430\u044f \u0440\u0430\u0434\u043e\u0441\u0442\u044c \u2014 \u043a\u0440\u044b\u043c\u0447\u0430\u043d\u0435 \u043e\u0442 \u0432\u0441\u0435\u0439 \u0434\u0443\u0448\u0438 \u043f\u0440\u0430\u0437\u0434\u043d\u0443\u044e\u0442 \u043d\u0430\u0441\u0442\u0443\u043f\u0438\u0432\u0448\u0435\u0435 \u0420\u043e\u0436\u0434\u0435\u0441\u0442\u0432\u043e \u0421\u0435\u0433\u043e\u0434\u043d\u044f \u043d\u0430\u0441\u0442\u0443\u043f\u0438\u043b \u0441\u0432\u0435\u0442\u043b\u044b\u0439 \u0445\u0440\u0438\u0441\u0442\u0438\u0430\u043d\u0441\u043a\u0438\u0439 \u043f\u0440\u0430\u0437\u0434\u043d\u0438\u043a \u2014 \u0420\u043e\u0436\u0434\u0435\u0441\u0442\u0432\u043e \u0425\u0440\u0438\u0441\u0442\u043e\u0432\u043e. \u041f\u043e \u0432\u0441\u0435\u0439 \u0441\u0442\u0440\u0430\u043d\u0435 \u0432 \u0445\u0440\u0430\u043c\u0430\u0445 \u043f\u0440\u043e\u0448\u043b\u0438 \u0431\u043e\u0433\u043e\u0441\u043b\u0443\u0436\u0435\u043d\u0438\u044f, \u0441\u043e\u0431\u0440\u0430\u0432\u0448\u0438\u0435 \u0432\u0435\u0440\u0443\u044e\u0449\u0438\u0445, \u043d\u0435 \u0441\u0442\u0430\u043b \u0438\u0441\u043a\u043b\u044e\u0447\u0435\u043d\u0438\u0435\u043c \u0438 \u041a\u0440\u044b\u043c. \u041d\u0430 \u044d\u0442\u0438\u0445 \u043a\u0430\u0434\u0440\u0430\u0445 \u2014 \u0430\u0442\u043c\u043e\u0441\u0444\u0435\u0440\u0430 \u0440\u043e\u0436\u0434\u0435\u0441\u0442\u0432\u0435\u043d\u0441\u043a\u043e\u0433\u043e \u0421\u0438\u043c\u0444\u0435\u0440\u043e\u043f\u043e\u043b\u044f, \u0433\u0434\u0435 \u0432 \u0441\u043e\u0431\u043e\u0440\u0435 \u043f\u0440\u043e\u0448\u043b\u0430 \u0441\u043b\u0443\u0436\u0431\u0430, \u0438 \u0425\u0435\u0440\u0441\u043e\u043d\u0435\u0441\u0430 \u0422\u0430\u0432\u0440\u0438\u0447\u0435\u0441\u043a\u043e\u0433\u043e, \u0433\u0434\u0435 \u0443\u0441\u0442\u0440\u043e\u0438\u043b\u0438 \u043f\u0440\u0430\u0437\u0434\u043d\u0438\u0447\u043d\u044b\u0435 \u043d\u0430\u0440\u043e\u0434\u043d\u044b\u0435 \u0433\u0443\u043b\u044f\u043d\u0438\u044f.\u041a\u043e\u0440\u0440\u0435\u0441\u043f\u043e\u043d\u0434\u0435\u043d\u0442 Readovka \u043f\u043e\u0433\u043e\u0432\u043e\u0440\u0438\u043b\u0430 \u0441 \u043b\u044e\u0434\u044c\u043c\u0438, \u043f\u0440\u0438\u0448\u0435\u0434\u0448\u0438\u043c\u0438 \u043d\u0430 \u043c\u0435\u0440\u043e\u043f\u0440\u0438\u044f\u0442\u0438\u044f \u2014 \u043c\u0430\u0441\u0442\u0435\u0440-\u043a\u043b\u0430\u0441\u0441\u044b \u0434\u043b\u044f \u0434\u0435\u0442\u0435\u0439 \u043f\u043e \u0440\u0430\u0441\u043a\u0440\u0430\u0448\u0438\u0432\u0430\u043d\u0438\u044e \u0430\u043d\u0433\u0435\u043b\u043e\u0447\u043a\u043e\u0432 \u0438 \u0438\u0441\u043f\u0435\u0447\u0435\u043d\u0438\u044e \u043f\u0440\u044f\u043d\u0438\u043a\u043e\u0432, \u0433\u0430\u0434\u0430\u043d\u0438\u044f \u0438 \u0443\u0433\u043e\u0449\u0435\u043d\u0438\u044f \u0433\u043b\u0438\u043d\u0442\u0432\u0435\u0439\u043d\u043e\u043c \u0434\u043b\u044f \u0432\u0437\u0440\u043e\u0441\u043b\u044b\u0445. \u0423 \u0432\u0441\u0435\u0445 \u0441\u0432\u0435\u0442\u043b\u043e\u0435, \u0440\u0430\u0434\u043e\u0441\u0442\u043d\u043e\u0435 \u043d\u0430\u0441\u0442\u0440\u043e\u0435\u043d\u0438\u0435 \u2014 \u0442\u0430\u043a\u043e\u0435 \u0436\u0435, \u043a\u0430\u043a \u0441\u0430\u043c \u043f\u0440\u0430\u0437\u0434\u043d\u0438\u043a, \u043a\u043e\u0433\u0434\u0430 \u0432 \u044d\u0442\u043e\u0442 \u043c\u0438\u0440 \u043f\u0440\u0438\u0448\u0435\u043b \u0425\u0440\u0438\u0441\u0442\u043e\u0441-\u0421\u043f\u0430\u0441\u0438\u0442\u0435\u043b\u044c.", "3": "<b>Total Posts:</b> 16<br><b>Date:</b> 2024-01-07 12:50:06+00:00<br><b>Author:</b> dmitrynikotin<br><b>Link:</b> https://t.me/s/dmitrynikotin/16095<br><b>Subscribers:</b> 642496<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u041d\u0435\u0438\u0437\u0432\u0435\u0441\u0442\u043d\u044b\u0435 \u0434\u0440\u043e\u043d\u044b \u043d\u0430\u0434 \u0431\u0430\u0437\u0430\u043c\u0438 \ud83c\udde9\ud83c\uddea\u0411\u0443\u043d\u0434\u0435\u0441\u0432\u0435\u0440\u0430 \u0441\u043b\u0435\u0434\u044f\u0442, \u043a\u0430\u043a \u0443\u0447\u0430\u0442\u0441\u044f \u0443\u043a\u0440\u0430\u0438\u043d\u0446\u044b \u2014 Bild.\u0415\u0436\u0435\u043d\u0435\u0434\u0435\u043b\u044c\u043d\u043e \u043d\u0435\u0438\u0437\u0432\u0435\u0441\u0442\u043d\u044b\u0435 \u0434\u0440\u043e\u043d\u044b \u043f\u0440\u043e\u043b\u0435\u0442\u0430\u044e\u0442 \u043d\u0430\u0434 \u0432\u043e\u0435\u043d\u043d\u044b\u043c\u0438 \u043f\u043e\u043b\u0438\u0433\u043e\u043d\u0430\u043c\u0438 \u0438 \u043a\u0430\u0437\u0430\u0440\u043c\u0430\u043c\u0438 \u0411\u0443\u043d\u0434\u0435\u0441\u0432\u0435\u0440\u0430, \u043d\u043e \u043f\u043e\u0439\u043c\u0430\u0442\u044c \u043d\u0438 \u043e\u0434\u043d\u043e\u0433\u043e \u0438\u0437 \u043d\u0438\u0445 \u043d\u0435 \u043c\u043e\u0433\u0443\u0442 \u0443\u0436\u0435 \u0431\u043e\u043b\u044c\u0448\u0435 \u0433\u043e\u0434\u0430.\u0414\u0435\u043f\u0443\u0442\u0430\u0442 \u0431\u0443\u043d\u0434\u0435\u0441\u0442\u0430\u0433\u0430 \u043e\u0442 \u0421\u0432\u043e\u0431\u043e\u0434\u043d\u043e\u0439 \u0434\u0435\u043c\u043e\u043a\u0440\u0430\u0442\u0438\u0447\u0435\u0441\u043a\u043e\u0439 \u043f\u0430\u0440\u0442\u0438\u0438, \u0447\u043b\u0435\u043d\u0430 \u043e\u0431\u043e\u0440\u043e\u043d\u043d\u043e\u0433\u043e \u043a\u043e\u043c\u0438\u0442\u0435\u0442\u0430 \u041c\u0430\u0440\u043a\u0443\u0441 \u0424\u0430\u0431\u0435\u0440 \u0441\u0447\u0438\u0442\u0430\u0435\u0442, \u0447\u0442\u043e \u044d\u0442\u043e \"\u0447\u0435\u0442\u043a\u043e \u0443\u043a\u0430\u0437\u044b\u0432\u0430\u0435\u0442 \u043d\u0430 \u0420\u043e\u0441\u0441\u0438\u044e\". \u0411\u0443\u043d\u0434\u0435\u0441\u0432\u0435\u0440 \u0442\u0430\u043a\u0436\u0435 \u043f\u043e\u0434\u043e\u0437\u0440\u0435\u0432\u0430\u0435\u0442, \u0447\u0442\u043e \u0437\u0430 \u043f\u0440\u043e\u043b\u0435\u0442\u043e\u043c \u0411\u041f\u041b\u0410 \u0441\u0442\u043e\u0438\u0442 \u041c\u043e\u0441\u043a\u0432\u0430, \u043d\u043e \u0434\u043e\u043a\u0430\u0437\u0430\u0442\u0435\u043b\u044c\u0441\u0442\u0432 \u044d\u0442\u043e\u0433\u043e \u043f\u043e\u043a\u0430 \u043d\u0435\u0442.\u0414\u043c\u0438\u0442\u0440\u0438\u0439 \u041d\u0438\u043a\u043e\u0442\u0438\u043d. \u041f\u043e\u0434\u043f\u0438\u0441\u0430\u0442\u044c\u0441\u044f!", "4": "<b>Total Posts:</b> 17<br><b>Date:</b> 2024-01-07 15:23:11+00:00<br><b>Author:</b> petrovtel<br><b>Link:</b> https://t.me/s/petrovtel/48926<br><b>Subscribers:</b> 494263<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u041f\u0440\u0435\u043c\u044c\u0435\u0440 \u0412\u0435\u043d\u0433\u0440\u0438\u0438 \u0412\u0438\u043a\u0442\u043e\u0440 \u041e\u0440\u0431\u0430\u043d \u043c\u043e\u0436\u0435\u0442 \u0441\u0442\u0430\u0442\u044c \u0433\u043b\u0430\u0432\u043e\u0439 \u0415\u0432\u0440\u043e\u0441\u043e\u0432\u0435\u0442\u0430, \u043f\u0438\u0448\u0435\u0442 Politico. \u0418\u0437\u0434\u0430\u043d\u0438\u0435 \u043e\u0442\u043c\u0435\u0447\u0430\u0435\u0442, \u0447\u0442\u043e \u043d\u044b\u043d\u0435\u0448\u043d\u0438\u0439 \u043f\u0440\u0435\u0434\u0441\u0435\u0434\u0430\u0442\u0435\u043b\u044c \u0415\u0432\u0440\u043e\u0441\u043e\u0432\u0435\u0442\u0430 \u0428\u0430\u0440\u043b\u044c \u041c\u0438\u0448\u0435\u043b\u044c \u043d\u0430\u043c\u0435\u0440\u0435\u043d \u0434\u043e\u0441\u0440\u043e\u0447\u043d\u043e \u0443\u0439\u0442\u0438 \u0441 \u043f\u043e\u0441\u0442\u0430 \u0438 \u0432\u044b\u0434\u0432\u0438\u043d\u0443\u0442\u044c \u0441\u0432\u043e\u044e \u043a\u0430\u043d\u0434\u0438\u0434\u0430\u0442\u0443\u0440\u0443 \u043d\u0430 \u0432\u044b\u0431\u043e\u0440\u0430\u0445 \u0432 \u0415\u0432\u0440\u043e\u043f\u0430\u0440\u043b\u0430\u043c\u0435\u043d\u0442 \u0432 \u0441\u0435\u0440\u0435\u0434\u0438\u043d\u0435 \u0438\u044e\u043b\u044f. \u0412 \u0441\u043b\u0443\u0447\u0430\u0435 \u0435\u0441\u043b\u0438 \u043e\u043d \u043e\u0434\u0435\u0440\u0436\u0438\u0442 \u043f\u043e\u0431\u0435\u0434\u0443, \u043b\u0438\u0434\u0435\u0440\u044b \u0441\u0442\u0440\u0430\u043d \u0415\u0421 \u0434\u043e\u043b\u0436\u043d\u044b \u0431\u0443\u0434\u0443\u0442 \u0431\u044b\u0441\u0442\u0440\u043e \u0434\u043e\u0433\u043e\u0432\u043e\u0440\u0438\u0442\u044c\u0441\u044f \u043e \u0435\u0433\u043e \u043f\u0440\u0435\u0435\u043c\u043d\u0438\u043a\u0435. \u0415\u0441\u043b\u0438 \u0432 \u0415\u0432\u0440\u043e\u0441\u043e\u044e\u0437\u0435 \u043d\u0435 \u043f\u0440\u0438\u0434\u0443\u0442 \u043a \u0441\u043e\u0433\u043b\u0430\u0441\u0438\u044e \u043f\u043e \u044d\u0442\u043e\u043c\u0443 \u0432\u043e\u043f\u0440\u043e\u0441\u0443, \u041e\u0440\u0431\u0430\u043d \u043a\u0430\u043a \u0433\u043b\u0430\u0432\u0430 \u043f\u0440\u0430\u0432\u0438\u0442\u0435\u043b\u044c\u0441\u0442\u0432\u0430 \u0412\u0435\u043d\u0433\u0440\u0438\u0438, \u043a\u043e\u0442\u043e\u0440\u0430\u044f \u0441 \u0438\u044e\u043b\u044f \u0441\u0442\u0430\u043d\u0435\u0442 \u043f\u0440\u0435\u0434\u0441\u0435\u0434\u0430\u0442\u0435\u043b\u044c\u0441\u0442\u0432\u0443\u044e\u0449\u0435\u0439 \u0432 \u0415\u0432\u0440\u043e\u0441\u043e\u0432\u0435\u0442\u0435, \u043d\u0430 \u043f\u043e\u043b\u0433\u043e\u0434\u0430 \u0441\u0442\u0430\u043d\u0435\u0442 \u0438.\u043e. \u0433\u043b\u0430\u0432\u044b \u0415\u0432\u0440\u043e\u0441\u043e\u0432\u0435\u0442\u0430. \u0421\u0442\u0440\u0430\u043d\u044b \u0415\u0421 \u0445\u043e\u0442\u044f\u0442 \u0438\u0437\u0431\u0435\u0436\u0430\u0442\u044c \u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u044f \u041e\u0440\u0431\u0430\u043d\u0430 \u0438\u0437-\u0437\u0430 \u0440\u0430\u0437\u043d\u043e\u0433\u043b\u0430\u0441\u0438\u0439 \u0441 \u043d\u0438\u043c, \u0432 \u0442\u043e\u043c \u0447\u0438\u0441\u043b\u0435 \u043f\u043e \u0432\u043e\u043f\u0440\u043e\u0441\u0443 \u043f\u043e\u0434\u0434\u0435\u0440\u0436\u043a\u0438 \u0423\u043a\u0440\u0430\u0438\u043d\u044b. \u041a\u041a \ud83d\udc00", "5": "<b>Total Posts:</b> 15<br><b>Date:</b> 2024-01-07 11:04:45+00:00<br><b>Author:</b> ssigny<br><b>Link:</b> https://t.me/s/ssigny/82713<br><b>Subscribers:</b> 510219<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \ud83d\udcf9\"\u041b\u0430\u043d\u0446\u0435\u0442\" 238-\u0439 \u0431\u0440\u0438\u0433\u0430\u0434\u044b \u0443\u043d\u0438\u0447\u0442\u043e\u0436\u0430\u0435\u0442 \u0433\u0430\u0443\u0431\u0438\u0446\u0443 \u0432\u0440\u0430\u0433\u0430 \u0420\u0430\u0441\u0447\u0435\u0442 \u0431\u0430\u0440\u0440\u0430\u0436\u0438\u0440\u0443\u044e\u0449\u0435\u0433\u043e \u0431\u043e\u0435\u043f\u0440\u0438\u043f\u0430\u0441\u0430 \"\u041b\u0430\u043d\u0446\u0435\u0442\" 238-\u0439 \u0430\u0440\u0442\u0438\u043b\u043b\u0435\u0440\u0438\u0439\u0441\u043a\u043e\u0439 \u0431\u0440\u0438\u0433\u0430\u0434\u044b \u043c\u0435\u0442\u043a\u0438\u043c \u043f\u043e\u043f\u0430\u0434\u0430\u043d\u0438\u0435\u043c \u0443\u043d\u0438\u0447\u0442\u043e\u0436\u0430\u0435\u0442 \u0431\u0443\u043a\u0441\u0438\u0440\u0443\u0435\u043c\u0443\u044e 122-\u043c\u043c \u0433\u0430\u0443\u0431\u0438\u0446\u0443 \"\u0414-30\" \u0412\u0421\u0423 \u043d\u0430 \u043e\u0433\u043d\u0435\u0432\u043e\u0439 \u043f\u043e\u0437\u0438\u0446\u0438\u0438.\u041f\u043e\u0434\u043f\u0438\u0441\u044b\u0432\u0430\u0439\u0442\u0435\u0441\u044c \u043d\u0430 \u0442\u0435\u043b\u0435\u0433\u0440\u0430\u043c\u043c \u043a\u0430\u043d\u0430\u043b \u041d\u0430\u0440\u043e\u0434\u043d\u0430\u044f \u043c\u0438\u043b\u0438\u0446\u0438\u044f \u0414\u041d\u0420, \u0447\u0442\u043e\u0431\u044b \u0443\u0432\u0438\u0434\u0435\u0442\u044c \u0432\u043e\u0439\u043d\u0443 \u043d\u0430\u0448\u0438\u043c\u0438 \u0433\u043b\u0430\u0437\u0430\u043c\u0438", "6": "<b>Total Posts:</b> 15<br><b>Date:</b> 2024-01-07 13:47:36+00:00<br><b>Author:</b> tobeor_official<br><b>Link:</b> https://t.me/s/ToBeOr_Official/14000<br><b>Subscribers:</b> 246972<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \"\u0411\u0443\u0434\u0435\u043c \u0434\u0443\u043c\u0430\u0442\u044c, \u043a\u0430\u043a \u043d\u0430\u043c \u0435\u0449\u0451 \u043f\u0440\u0438\u0432\u043b\u0435\u0447\u044c \u0432\u043d\u0438\u043c\u0430\u043d\u0438\u0435 \u043a \u043d\u0430\u0448\u0435\u0439 \u043f\u0440\u043e\u0431\u043b\u0435\u043c\u0435, \u043a \u043f\u0440\u043e\u0431\u043b\u0435\u043c\u0435 \u0432\u043e\u0439\u043d\u044b, \u043a\u043e\u0442\u043e\u0440\u0443\u044e \u0432\u0435\u0434\u0451\u0442 \u0420\u043e\u0441\u0441\u0438\u0439\u0441\u043a\u0430\u044f \u0424\u0435\u0434\u0435\u0440\u0430\u0446\u0438\u044f \u043f\u043e \u043e\u0442\u043d\u043e\u0448\u0435\u043d\u0438\u044e \u043a \u0423\u043a\u0440\u0430\u0438\u043d\u0435.\u0413\u043e\u043b\u043e\u0441\u043e\u0432\u0430\u0442\u044c \u0431\u0443\u0434\u0443 \u0437\u0430 \u043b\u044e\u0431\u043e\u0433\u043e, \u0442\u043e\u043b\u044c\u043a\u043e \u043d\u0435 \u0437\u0430 \u041f\u0443\u0442\u0438\u043d\u0430.\u041d\u0430\u0448\u0438 \u0441\u0435\u043c\u044c\u0438, \u0441\u0435\u043c\u044c\u0438 \u043c\u043e\u0431\u0438\u043b\u0438\u0437\u043e\u0432\u0430\u043d\u043d\u044b\u0445, \u0433\u0440\u0430\u0436\u0434\u0430\u043d\u0430\u043c\u0438 \u0420\u043e\u0441\u0441\u0438\u0439\u0441\u043a\u0438\u0439 \u0424\u0435\u0434\u0435\u0440\u0430\u0446\u0438\u0438 \u043d\u0435 \u044f\u0432\u043b\u044f\u044e\u0442\u0441\u044f. \u041d\u0430\u0432\u0435\u0440\u043d\u043e\u0435, \u044d\u0442\u043e \u043d\u0435 \u043d\u0430\u0448 \u0433\u043e\u0434, \u0438\u043b\u0438 \u043d\u0430\u0441 \u0443\u0436\u0435 \"\u043e\u0431\u043d\u0443\u043b\u0438\u043b\u0438\", \u0441\u043f\u0438\u0441\u0430\u043b\u0438 \u0441\u043e \u0441\u0447\u0435\u0442\u043e\u0432\", - \u0430\u043a\u0442\u0438\u0432\u0438\u0441\u0442\u043a\u0430 \u041c\u0430\u0440\u0438\u044f \u0410\u043d\u0434\u0440\u0435\u0435\u0432\u0430.\u0420\u043e\u0441\u0441\u0438\u0439\u0441\u043a\u0438\u0435 \u0436\u0451\u043d\u044b, \u0443\u0447\u0430\u0441\u0442\u043d\u0438\u0446\u044b \u0434\u0432\u0438\u0436\u0435\u043d\u0438\u044f \"\u041f\u0443\u0442\u044c \u0434\u043e\u043c\u043e\u0439\" \u043f\u0440\u043e\u0432\u043e\u0434\u044f\u0442 \u043f\u0438\u043a\u0435\u0442\u044b, \u0440\u0430\u0441\u043a\u043b\u0435\u0438\u0432\u0430\u044e\u0442 \u043b\u0438\u0441\u0442\u043e\u0432\u043a\u0438 \u0438 \u0440\u0430\u0441\u0448\u0438\u0440\u044f\u044e\u0442 \u0441\u0432\u043e\u044e \u0434\u0435\u044f\u0442\u0435\u043b\u044c\u043d\u043e\u0441\u0442\u044c.\u0412\u0438\u0434\u0435\u043e: SOTAvision", "7": "<b>Total Posts:</b> 24<br><b>Date:</b> 2024-01-07 08:12:01+00:00<br><b>Author:</b> rlz_the_kraken<br><b>Link:</b> https://t.me/s/rlz_the_kraken/63060<br><b>Subscribers:</b> 259194<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \ud83e\udd21\"\u0423 \u0442\u0435\u0445, \u043a\u0442\u043e \u0432 \u0430\u0440\u043c\u0438\u0438 \u2014 \u0448\u0430\u043d\u0441\u043e\u0432 \u0432\u044b\u0436\u0438\u0442\u044c \u0431\u043e\u043b\u044c\u0448\u0435, \u0447\u0435\u043c \u0443 \u0442\u0435\u0445, \u043a\u0442\u043e \u043f\u044b\u0442\u0430\u0435\u0442\u0441\u044f \u043e\u0442\u043a\u043e\u0441\u0438\u0442\u044c\"\u0417\u0430\u043c\u0440\u0443\u043a\u043e\u0432\u043e\u0434\u0438\u0442\u0435\u043b\u044f \u0446\u0435\u043d\u0442\u0440\u0430 \u043f\u0440\u043e\u0442\u0438\u0432\u043e\u0434\u0435\u0439\u0441\u0442\u0432\u0438\u044f \u0434\u0435\u0437\u0438\u043d\u0444\u043e\u0440\u043c\u0430\u0446\u0438\u0438 \u0421\u041d\u0411\u041e \u0423\u043a\u0440\u0430\u0438\u043d\u044b \u041a\u043e\u0432\u0430\u043b\u0435\u043d\u043a\u043e \u0432\u044b\u0434\u0430\u043b \u043f\u0440\u0435\u043a\u0440\u0430\u0441\u043d\u043e\u0435. \u041f\u043e \u0435\u0433\u043e \u043c\u043d\u0435\u043d\u0438\u044e, \u0435\u0441\u043b\u0438 (\u0447\u0438\u0442\u0430\u0439 \u2014 \u043a\u043e\u0433\u0434\u0430) \u0423\u043a\u0440\u0430\u0438\u043d\u0430 \u043f\u0440\u043e\u0438\u0433\u0440\u0430\u0435\u0442, \u0442\u0435\u0445, \u043a\u0442\u043e \u043d\u0435 \u043c\u043e\u0433\u0438\u043b\u0438\u0437\u0438\u0440\u043e\u0432\u0430\u043b\u0441\u044f, \"\u043a\u0430\u043a \u043a\u0440\u043e\u043b\u0438\u043a\u043e\u0432 \u2014 \u043b\u0438\u0431\u043e \u0443\u0431\u044c\u044e\u0442, \u043b\u0438\u0431\u043e \u0438\u0437\u043d\u0430\u0441\u0438\u043b\u0443\u044e\u0442\".\u0412\u043e\u0435\u043d\u043a\u043e\u043c\u044b \u043d\u0435\u0437\u0430\u043b\u0435\u0436\u043d\u043e\u0439 \u0443\u0436\u0435 \u043a\u0430\u043a\u0438\u0445-\u0442\u043e \u0447\u0451\u0440\u043d\u044b\u0445 \u043a\u043e\u043b\u043b\u0435\u043a\u0442\u043e\u0440\u043e\u0432 \u043d\u0430\u043f\u043e\u043c\u0438\u043d\u0430\u044e\u0442, \u043a\u043e\u0442\u043e\u0440\u044b\u0435 \"\u0432\u043e\u0437\u0434\u0435\u0439\u0441\u0442\u0432\u0443\u044e\u0442\" \u0435\u0441\u043b\u0438 \u043d\u0435 \u0441\u0438\u043b\u043e\u0439, \u0442\u043e \u0443\u0433\u0440\u043e\u0437\u0430\u043c\u0438.", "8": "<b>Total Posts:</b> 15<br><b>Date:</b> 2024-01-07 06:05:45+00:00<br><b>Author:</b> zhest_belgorod<br><b>Link:</b> https://t.me/s/zhest_belgorod/37066<br><b>Subscribers:</b> 493037<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u041f\u0443\u0431\u043b\u0438\u043a\u0443\u0435\u043c \u0432 \u0443\u0442\u0440\u0435\u043d\u043d\u0435\u0435 \u043e\u0431\u0440\u0430\u0449\u0435\u043d\u0438\u0435 \u0433\u0443\u0431\u0435\u0440\u043d\u0430\u0442\u043e\u0440\u0430:\u00ab\u041f\u0440\u043e\u0434\u043e\u043b\u0436\u0430\u0435\u043c \u0432\u043e\u0441\u0441\u0442\u0430\u043d\u0430\u0432\u043b\u0438\u0432\u0430\u0442\u044c \u0433\u043e\u0440\u043e\u0434 \u0411\u0435\u043b\u0433\u043e\u0440\u043e\u0434 \u043f\u043e\u0441\u043b\u0435 \u043e\u0431\u0441\u0442\u0440\u0435\u043b\u0430 \u0441\u043e \u0441\u0442\u043e\u0440\u043e\u043d\u044b \u0412\u0421\u0423. 1900 \u043a\u0432\u0430\u0434\u0440\u0430\u0442\u043d\u044b\u0445 \u043c\u0435\u0442\u0440\u043e\u0432 \u043e\u0441\u0442\u0435\u043a\u043b\u0435\u043d\u0438\u044f \u0443\u0436\u0435 \u0432\u043e\u0441\u0441\u0442\u0430\u043d\u043e\u0432\u043b\u0435\u043d\u043e. \u0411\u043e\u043b\u0435\u0435 400 \u043a\u0432\u0430\u0434\u0440\u0430\u0442\u043d\u044b\u0445 \u043c\u0435\u0442\u0440\u043e\u0432 \u043a\u0440\u043e\u0432\u0435\u043b\u044c\u043d\u044b\u0445 \u0440\u0430\u0431\u043e\u0442. \u0420\u0430\u0431\u043e\u0442\u044b \u043f\u0440\u043e\u0434\u043e\u043b\u0436\u0430\u044e\u0442\u0441\u044f. \u042f \u0443\u0432\u0435\u0440\u0435\u043d, \u0447\u0442\u043e \u0431\u044b\u0441\u0442\u0440\u043e \u0438\u0445 \u0437\u0430\u0432\u0435\u0440\u0448\u0438\u043c.\u2800\u041f\u043e \u043d\u0430\u0448\u0438\u043c 68 \u0440\u0430\u043d\u0435\u043d\u044b\u043c, \u043a\u043e\u0442\u043e\u0440\u044b\u0435 \u043d\u0430\u0445\u043e\u0434\u044f\u0442\u0441\u044f \u0432 \u0431\u043e\u043b\u044c\u043d\u0438\u0446\u0430\u0445 \u0411\u0435\u043b\u0433\u043e\u0440\u043e\u0434\u0430 \u0438 \u041c\u043e\u0441\u043a\u0432\u044b (1 \u0432\u044b\u043f\u0438\u0441\u0430\u043d \u0432\u0447\u0435\u0440\u0430) - 4 \u0432\u0437\u0440\u043e\u0441\u043b\u044b\u0445 \u0447\u0435\u043b\u043e\u0432\u0435\u043a\u0430 \u0438 4 \u0440\u0435\u0431\u0435\u043d\u043a\u0430 \u0432 \u0431\u043e\u043b\u044c\u043d\u0438\u0446\u0430\u0445 \u041c\u043e\u0441\u043a\u0432\u044b \u043f\u0435\u0440\u0435\u0432\u0435\u0434\u0435\u043d\u044b \u0438\u0437 \u0440\u0435\u0430\u043d\u0438\u043c\u0430\u0446\u0438\u0438 \u0432 \u043e\u0431\u044b\u0447\u043d\u044b\u0435 \u043f\u0430\u043b\u0430\u0442\u044b. \u042f \u0443\u0432\u0435\u0440\u0435\u043d, \u0447\u0442\u043e \u0443\u0436\u0435 \u0441\u043e\u0432\u0441\u0435\u043c \u0441\u043a\u043e\u0440\u043e \u0432\u0441\u0435 \u043e\u043d\u0438 \u0432\u0435\u0440\u043d\u0443\u0442\u0441\u044f \u043a \u0441\u0432\u043e\u0438\u043c \u0431\u043b\u0438\u0437\u043a\u0438\u043c \u0438 \u0440\u043e\u0434\u043d\u044b\u043c, \u043a\u043e\u0442\u043e\u0440\u044b\u0435 \u0437\u0430 \u043d\u0438\u0445 \u043e\u0447\u0435\u043d\u044c \u043f\u0435\u0440\u0435\u0436\u0438\u0432\u0430\u044e\u0442.\u2800\u0412\u0447\u0435\u0440\u0430 \u043d\u0430 \u041f\u043e\u0447\u0442\u043e\u0432\u043e\u0439 \u043a\u043e \u043c\u043d\u0435 \u043f\u043e\u0434\u043e\u0448\u043b\u0430 \u0436\u0435\u043d\u0449\u0438\u043d\u0430, \u043f\u0440\u0435\u0434\u0441\u0442\u0430\u0432\u0438\u043b\u0430\u0441\u044c \u0438 \u0441\u043a\u0430\u0437\u0430\u043b\u0430, \u0447\u0442\u043e \u043e\u043d\u0430 \u043c\u0430\u043c\u0430 \u0442\u0440\u043e\u0438\u0445 \u0434\u0435\u0442\u0435\u0439. \u041a\u043e\u043d\u0435\u0447\u043d\u043e, \u043e\u0447\u0435\u043d\u044c \u043f\u0435\u0440\u0435\u0436\u0438\u0432\u0430\u0435\u0442, \u0447\u0442\u043e \u0441 9 \u044f\u043d\u0432\u0430\u0440\u044f, \u043a\u043e\u0433\u0434\u0430 \u0432\u0441\u0435 \u0432\u044b\u0439\u0434\u0443\u0442 \u0443\u0436\u0435 \u043d\u0430 \u0440\u0430\u0431\u043e\u0442\u0443, \u0434\u0435\u0442\u0438 \u043e\u0441\u0442\u0430\u043d\u0443\u0442\u0441\u044f \u0432 \u0441\u0432\u044f\u0437\u0438 \u0441 \u043f\u0440\u043e\u0434\u043b\u0435\u043d\u043d\u044b\u043c\u0438 \u043a\u0430\u043d\u0438\u043a\u0443\u043b\u0430\u043c\u0438 \u0434\u043e\u043c\u0430. \u0420\u043e\u0434\u0438\u0442\u0435\u043b\u0438 \u0431\u0443\u0434\u0443\u0442 \u043f\u0435\u0440\u0435\u0436\u0438\u0432\u0430\u0442\u044c \u0437\u0430 \u0442\u043e, \u043a\u0430\u043a \u043e\u043d\u0438 \u0441\u0435\u0431\u044f \u0447\u0443\u0432\u0441\u0442\u0432\u0443\u044e\u0442, \u043a\u0442\u043e \u0438\u043c \u043f\u043e\u043c\u043e\u0436\u0435\u0442, \u0435\u0441\u043b\u0438 \u0432\u0434\u0440\u0443\u0433 \u0432\u043e\u0437\u043d\u0438\u043a\u043d\u0435\u0442 \u0441\u043b\u043e\u0436\u043d\u0430\u044f \u0441\u0438\u0442\u0443\u0430\u0446\u0438\u044f. \u041c\u043e\u0435 \u043f\u0440\u0435\u0434\u043b\u043e\u0436\u0435\u043d\u0438\u0435: \u043c\u044b \u0433\u043e\u0442\u043e\u0432\u044b \u0441\u043e\u0431\u0440\u0430\u0442\u044c \u0433\u0440\u0443\u043f\u043f\u044b, \u0441\u0444\u043e\u0440\u043c\u0438\u0440\u043e\u0432\u0430\u0442\u044c \u043d\u0430\u0448\u0438\u0445 \u0434\u0435\u0442\u0435\u0439 \u0438\u0437 \u0411\u0435\u043b\u0433\u043e\u0440\u043e\u0434\u0430, \u0447\u0442\u043e\u0431\u044b \u043e\u0442\u043f\u0440\u0430\u0432\u0438\u0442\u044c \u0438\u0445 \u0432 \u0437\u0430\u0433\u043e\u0440\u043e\u0434\u043d\u044b\u0435 \u043b\u0430\u0433\u0435\u0440\u044f \u0434\u0440\u0443\u0433\u0438\u0445 \u0440\u0435\u0433\u0438\u043e\u043d\u043e\u0432. \u0415\u0441\u0442\u044c \u043f\u0440\u0435\u0434\u043b\u043e\u0436\u0435\u043d\u0438\u044f \u043e\u0442 \u043c\u043e\u0438\u0445 \u043a\u043e\u043b\u043b\u0435\u0433 \u0438\u0437 \u0447\u0438\u0441\u043b\u0430 \u0433\u0443\u0431\u0435\u0440\u043d\u0430\u0442\u043e\u0440\u043e\u0432. \u041d\u0430\u043f\u043e\u043c\u043d\u044e, \u0447\u0442\u043e \u043c\u044b \u0432\u044b\u0432\u043e\u0437\u0438\u043b\u0438 \u043d\u0430\u0448\u0438\u0445 \u0434\u0435\u0442\u0435\u0439 \u0438\u0437 \u043f\u0440\u0438\u0433\u0440\u0430\u043d\u0438\u0447\u043d\u044b\u0445 \u0442\u0435\u0440\u0440\u0438\u0442\u043e\u0440\u0438\u0439 \u0438 \u043b\u0435\u0442\u043e\u043c. \u041e\u0442\u0432\u043e\u0437\u0438\u043b\u0438 \u0434\u0435\u0442\u0435\u0439 \u0438\u0437 \u0428\u0435\u0431\u0435\u043a\u0438\u043d\u0441\u043a\u043e\u0433\u043e \u0438 \u0413\u0440\u0430\u0439\u0432\u043e\u0440\u043e\u043d\u0441\u043a\u043e\u0433\u043e \u043e\u043a\u0440\u0443\u0433\u043e\u0432. \u0423 \u043d\u0430\u0441 \u0432 \u0441\u0435\u0440\u0435\u0434\u0438\u043d\u0435 \u044f\u043d\u0432\u0430\u0440\u044f \u043d\u0430\u0447\u043d\u0451\u0442 \u0440\u0430\u0431\u043e\u0442\u0430\u0442\u044c \u043d\u0430\u0448 \u043a\u0440\u0443\u0433\u043b\u043e\u0433\u043e\u0434\u0438\u0447\u043d\u044b\u0439 \u0441\u0430\u043d\u0430\u0442\u043e\u0440\u0438\u0439 \u00ab\u0411\u0440\u0438\u0433\u0430\u043d\u0442\u0438\u043d\u0430 \"\u0411\u0435\u043b\u043e\u0433\u043e\u0440\u044c\u0435\"\u00bb \u0432 \u041a\u0440\u044b\u043c\u0443. \u0415\u0441\u043b\u0438 \u0445\u043e\u0442\u0438\u0442\u0435, \u044f \u0441\u0435\u0439\u0447\u0430\u0441 \u043e\u0431\u0440\u0430\u0449\u0430\u044e\u0441\u044c \u043a \u0440\u043e\u0434\u0438\u0442\u0435\u043b\u044f\u043c \u0433\u043e\u0440\u043e\u0434\u0430 \u0411\u0435\u043b\u0433\u043e\u0440\u043e\u0434\u0430, \u0442\u043e, \u043f\u043e\u0436\u0430\u043b\u0443\u0439\u0441\u0442\u0430, \u043e\u0431\u0440\u0430\u0449\u0430\u0439\u0442\u0435\u0441\u044c \u0432 \u0430\u0434\u043c\u0438\u043d\u0438\u0441\u0442\u0440\u0430\u0446\u0438\u044e \u0433\u043e\u0440\u043e\u0434\u0430, \u0432 \u041c\u0438\u043d\u0438\u0441\u0442\u0435\u0440\u0441\u0442\u0432\u043e \u043e\u0431\u0440\u0430\u0437\u043e\u0432\u0430\u043d\u0438\u044f, \u043a \u0434\u0438\u0440\u0435\u043a\u0442\u043e\u0440\u0430\u043c \u0448\u043a\u043e\u043b. \u041c\u044b \u0434\u0435\u043b\u0430\u0435\u043c \u0432\u0441\u0435, \u0447\u0442\u043e \u043e\u0442 \u043d\u0430\u0441 \u0437\u0430\u0432\u0438\u0441\u0438\u0442, \u0447\u0442\u043e\u0431\u044b \u043f\u043e\u043c\u043e\u0447\u044c \u043d\u0430\u0448\u0438\u043c \u0434\u0435\u0442\u044f\u043c. \u0416\u0434\u0443 \u0432\u0430\u0448\u0435\u0433\u043e \u043c\u043d\u0435\u043d\u0438\u044f, \u0447\u0442\u043e\u0431\u044b \u0441\u043e\u0432\u043c\u0435\u0441\u0442\u043d\u043e \u0441 \u0432\u0430\u043c\u0438 \u0440\u0435\u0448\u0430\u0442\u044c \u0442\u0435 \u043f\u0440\u043e\u0431\u043b\u0435\u043c\u044b, \u043a\u043e\u0442\u043e\u0440\u044b\u0435 \u0441\u0435\u0439\u0447\u0430\u0441 \u0441\u0442\u043e\u044f\u0442 \u043f\u0435\u0440\u0435\u0434 \u043d\u0430\u043c\u0438\u00bb, \u2013 \u0441\u043e\u043e\u0431\u0449\u0438\u043b \u0412\u044f\u0447\u0435\u0441\u043b\u0430\u0432 \u0413\u043b\u0430\u0434\u043a\u043e\u0432. \ud83d\udd25 \u0416\u0435\u0441\u0442\u044c \u0411\u0435\u043b\u0433\u043e\u0440\u043e\u0434 - \u043f\u043e\u0434\u043f\u0438\u0441\u0430\u0442\u044c\u0441\u044f", "9": "<b>Total Posts:</b> 17<br><b>Date:</b> 2024-01-07 09:26:56+00:00<br><b>Author:</b> rtrdonetsk<br><b>Link:</b> https://t.me/s/RtrDonetsk/22256<br><b>Subscribers:</b> 255766<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \ud83d\udd34\ud83d\udd34\ud83d\udd34\ud83d\udd34\ud83d\udd34\u041e \u043f\u043e\u0441\u043b\u0435\u0434\u0441\u0442\u0432\u0438\u044f\u0445 \u0440\u0430\u043a\u0435\u0442\u043d\u043e\u0433\u043e \u0443\u0434\u0430\u0440\u0430 \u0412\u0424\u0423 \u043f\u043e \u0431\u043e\u043b\u044c\u043d\u0438\u0446\u0435 \u0432 \u0414\u043e\u043d\u0435\u0446\u043a\u0435\u0412 \u044d\u0444\u0438\u0440\u0435 \u0442\u0435\u043b\u0435\u043a\u0430\u043d\u0430\u043b\u0430\u23eb\u23eb\u23eb\u23eb\u23eb\u0440\u0430\u0441\u0441\u043a\u0430\u0437\u0430\u043b\u0430 \u043a\u043e\u0440\u0440\u0435\u0441\u043f\u043e\u043d\u0434\u0435\u043d\u0442 \u0412\u0435\u0441\u0442\u0438.\u0414\u043e\u043d\u0435\u0446\u043a \u041e\u043b\u044c\u0433\u0430 \u041b\u0443\u043a\u044c\u044f\u043d\u0447\u0435\u043d\u043a\u043e.\ud83d\udcf0 \u0412\u0435\u0441\u0442\u0438.\u0414\u043e\u043d\u0435\u0446\u043a | \u041f\u0440\u0435\u0434\u043b\u043e\u0436\u0438\u0442\u044c \u043d\u043e\u0432\u043e\u0441\u0442\u044c"};

    function displayClusterText() {
        var selectedLabel = document.getElementById("clusterSelector").value;
        var details = clusterDetails[selectedLabel];
        var textDiv = document.getElementById("clusterTextDisplay");
        textDiv.innerHTML = '<p>' + details + '</p>';
        textDiv.classList.remove('hidden');
    }
</script>
