---
layout: post
title: "Russia Telegram Analysis - 2024-10-04"
author: "Dmytro Bukhanevych"
categories: analysis
tags: [telegram, analysis]
image: pawel-czerwinski-s6Nn0Q_ARWs-unsplash.jpg
permalink: "/analysis/russia-telegram-analysis-2024-10-04"
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
<p>Загалом було проаналізовано 9839 постів у Telegram за 03.10.2024. Було відстежено активність 123 найбільш популярних Telegram каналів у Росії. Після попередньої обробки, фільтрування за ключовими словами, кластеризації та зменшення шуму, 1401 текстів було проаналізовано у крайньому звітному періоді.</p>
<!-- Embedding Main Plotly Visualization -->
<div class="wide-iframe-container">
    <iframe src="{{site.baseurl}}/visualizations/2024-10-04/fig_topics_time.html" height="850"></iframe>
</div>


<h2>Cluster Text</h2>

<!-- Dropdown to select a cluster -->
<select id="clusterSelector" onchange="displayClusterText()">
<option value="0">Cluster 0</option><option value="1">Cluster 1</option><option value="2">Cluster 2</option><option value="3">Cluster 3</option><option value="4">Cluster 4</option><option value="5">Cluster 5</option><option value="6">Cluster 6</option><option value="7">Cluster 7</option><option value="8">Cluster 8</option>
</select>

<!-- Display area for the selected cluster's text -->
<div id="clusterTextDisplay" class="hidden"></div>

<script type="text/javascript">
    var clusterDetails = {"0": "<b>Total Posts:</b> 588<br><b>Date:</b> 2024-10-03 19:59:01+00:00<br><b>Author:</b> rvvoenkor<br><b>Link:</b> https://t.me/s/RVvoenkor/78123<br><b>Subscribers:</b> 1620127<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u203c\ufe0f\ud83c\uddf7\ud83c\uddfa \u041f\u0435\u0440\u0432\u044b\u0435 \u043a\u0430\u0434\u0440\u044b \u0438\u0437 \u043e\u0441\u0432\u043e\u0431\u043e\u0436\u0434\u0451\u043d\u043d\u043e\u0433\u043e \u0423\u0433\u043b\u0435\u0434\u0430\u0440\u0430.\u25aa\ufe0f\u0421\u044a\u0451\u043c\u043a\u0430 \u0431\u043e\u0439\u0446\u043e\u0432 37 \u043c\u043e\u0442\u043e\u0441\u0442\u0440\u0435\u043b\u043a\u043e\u0432\u043e\u0439 \u0431\u0440\u0438\u0433\u0430\u0434\u044b 36 \u0430\u0440\u043c\u0438\u0438 \u0433\u0440\u0443\u043f\u043f\u0438\u0440\u043e\u0432\u043a\u0438 \"\u0412\u043e\u0441\u0442\u043e\u043a\".\u25aa\ufe0f\u0412\u0437\u044f\u0442\u0438\u0435 \u043f\u043e\u0434 \u043a\u043e\u043d\u0442\u0440\u043e\u043b\u044c \u0423\u0433\u043b\u0435\u0434\u0430\u0440\u0430 \u0432 \u0414\u041d\u0420 \u0432\u0430\u0436\u043d\u043e \u043a\u0430\u043a \u0434\u043b\u044f \u0437\u0430\u0449\u0438\u0442\u044b \u043f\u043e\u0434\u0445\u043e\u0434\u043e\u0432 \u043a \u041c\u0430\u0440\u0438\u0443\u043f\u043e\u043b\u044e, \u0442\u0430\u043a \u0438 \u0434\u043b\u044f \u043e\u0441\u0432\u043e\u0431\u043e\u0436\u0434\u0435\u043d\u0438\u044f \u041a\u0443\u0440\u0430\u0445\u043e\u0432\u0430.\u25aa\ufe0f \u041e\u043a\u0440\u0435\u0441\u0442\u043d\u043e\u0441\u0442\u0438 \u0433\u043e\u0440\u043e\u0434\u0430 \u0437\u0430\u0432\u0430\u043b\u0435\u043d\u044b \u0441\u043e\u0442\u043d\u044f\u043c\u0438 \u0442\u0440\u0443\u043f\u043e\u0432 \u0431\u043e\u0435\u0432\u0438\u043a\u043e\u0432 \u0412\u0421\u0423.\u25aa\ufe0f\u0422\u0435\u043c \u0432\u0440\u0435\u043c\u0435\u043d\u0435\u043c \u0440\u043e\u0441\u0441\u0438\u0439\u0441\u043a\u0438\u0435 \u0432\u043e\u0439\u0441\u043a\u0430 \u0440\u0432\u0443\u0442\u0441\u044f \u0432\u043f\u0435\u0440\u0451\u0434.t.me/RVvoenkor", "1": "<b>Total Posts:</b> 188<br><b>Date:</b> 2024-10-03 16:19:56+00:00<br><b>Author:</b> zhest_belgorod<br><b>Link:</b> https://t.me/s/zhest_belgorod/50504<br><b>Subscribers:</b> 705850<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u2757\ufe0f\u0412 \u0440\u0430\u0439\u043e\u043d\u0435 \u041a\u0443\u0440\u0447\u0430\u0442\u043e\u0432\u0430 \u041a\u0443\u0440\u0441\u043a\u043e\u0439 \u043e\u0431\u043b\u0430\u0441\u0442\u0438 \u0441\u0440\u0435\u0434\u0441\u0442\u0432\u0430\u043c\u0438 \u0420\u042d\u0411 \u043f\u043e\u0434\u0430\u0432\u043b\u0435\u043d \u0443\u043a\u0440\u0430\u0438\u043d\u0441\u043a\u0438\u0439 \u0411\u041f\u041b\u0410 \u0441\u0430\u043c\u043e\u043b\u0435\u0442\u043d\u043e\u0433\u043e \u0442\u0438\u043f\u0430. \u00ab\u0412 \u0440\u0435\u0437\u0443\u043b\u044c\u0442\u0430\u0442\u0435 \u0435\u0433\u043e \u043f\u0430\u0434\u0435\u043d\u0438\u044f \u043f\u0440\u043e\u0438\u0437\u043e\u0448\u043b\u0438 \u0432\u0437\u0440\u044b\u0432\u044b \u0432 \u0445\u043e\u0437\u043f\u043e\u0441\u0442\u0440\u043e\u0439\u043a\u0435, \u043d\u0435 \u0438\u043c\u0435\u044e\u0449\u0435\u0439 \u043e\u0442\u043d\u043e\u0448\u0435\u043d\u0438\u044f \u043a \u041a\u0443\u0440\u0441\u043a\u043e\u0439 \u0410\u042d\u0421. \u042d\u043a\u0441\u0442\u0440\u0435\u043d\u043d\u044b\u0435 \u0441\u043b\u0443\u0436\u0431\u044b \u043d\u0430 \u043c\u0435\u0441\u0442\u0435\u00bb, \u2014 \u0441\u043e\u043e\u0431\u0449\u0438\u043b \u0433\u0443\u0431\u0435\u0440\u043d\u0430\u0442\u043e\u0440 \u0410\u043b\u0435\u043a\u0441\u0435\u0439 \u0421\u043c\u0438\u0440\u043d\u043e\u0432.\u2755 \u0416\u0435\u0441\u0442\u044c \u0411\u0435\u043b\u0433\u043e\u0440\u043e\u0434 - \u043f\u043e\u0434\u043f\u0438\u0441\u0430\u0442\u044c\u0441\u044f", "2": "<b>Total Posts:</b> 125<br><b>Date:</b> 2024-10-03 03:56:04+00:00<br><b>Author:</b> dmitrynikotin<br><b>Link:</b> https://t.me/s/dmitrynikotin/24501<br><b>Subscribers:</b> 716009<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u0418\u0437\u0440\u0430\u0438\u043b\u044c \u0440\u0430\u0441\u0441\u043c\u0430\u0442\u0440\u0438\u0432\u0430\u0435\u0442 \u0432\u043e\u0437\u043c\u043e\u0436\u043d\u043e\u0441\u0442\u044c \u043d\u0430\u043f\u0430\u0434\u0435\u043d\u0438\u044f \u043d\u0430 \u0438\u0440\u0430\u043d\u0441\u043a\u0438\u0435 \u043e\u0431\u044a\u0435\u043a\u0442\u044b \u0432 \u0419\u0435\u043c\u0435\u043d\u0435 \u0438\u043b\u0438 \u0421\u0438\u0440\u0438\u0438 \u0432\u043c\u0435\u0441\u0442\u043e \u043e\u0431\u044a\u0435\u043a\u0442\u043e\u0432 \u0432 \u0418\u0440\u0430\u043d\u0435.\u041e\u0431 \u044d\u0442\u043e\u043c \u043f\u0438\u0448\u0435\u0442 Politico.\u0418\u0437\u0434\u0430\u043d\u0438\u0435 \u0441\u043e\u043e\u0431\u0449\u0430\u0435\u0442, \u0447\u0442\u043e \u0411\u0430\u0439\u0434\u0435\u043d \u043e\u0447\u0435\u043d\u044c \u0437\u043e\u043b \u043d\u0430 \u0434\u0435\u0439\u0441\u0442\u0432\u0438\u044f \u041d\u0435\u0442\u0430\u043d\u044c\u044f\u0445\u0443, \u043d\u043e \u043d\u0438\u0447\u0435\u0433\u043e \u043d\u0435 \u043c\u043e\u0436\u0435\u0442 \u043f\u043e\u0434\u0435\u043b\u0430\u0442\u044c, \u043f\u043e\u0441\u043a\u043e\u043b\u044c\u043a\u0443 \u0418\u0437\u0440\u0430\u0438\u043b\u044c \u043f\u043e\u043a\u0430\u0437\u044b\u0432\u0430\u0435\u0442 \u0433\u0440\u0430\u043d\u0438\u0446\u044b \u0435\u0433\u043e \u0432\u043b\u0438\u044f\u043d\u0438\u044f \u0438 \u0432\u044b\u0441\u0442\u0430\u0432\u043b\u044f\u0435\u0442 \u043f\u0440\u0435\u0437\u0438\u0434\u0435\u043d\u0442\u0430 \u0421\u0428\u0410 \u00ab\u0445\u0440\u043e\u043c\u043e\u0439 \u0443\u0442\u043a\u043e\u0439\u00bb.\ud83d\udcf1\u0414\u043c\u0438\u0442\u0440\u0438\u0439 \u041d\u0438\u043a\u043e\u0442\u0438\u043d. \u041f\u043e\u0434\u043f\u0438\u0441\u0430\u0442\u044c\u0441\u044f!", "3": "<b>Total Posts:</b> 43<br><b>Date:</b> 2024-10-03 14:35:34+00:00<br><b>Author:</b> kontext_channel<br><b>Link:</b> https://t.me/s/kontext_channel/42411<br><b>Subscribers:</b> 925702<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u0412\u043b\u0430\u0434\u0438\u043c\u0438\u0440 \u041f\u0443\u0442\u0438\u043d \u043f\u043e\u0434\u0434\u0435\u0440\u0436\u0430\u043b \u0438\u0434\u0435\u044e \u0440\u0430\u0441\u043f\u0440\u043e\u0441\u0442\u0440\u0430\u043d\u0438\u0442\u044c \u043f\u0440\u043e\u0435\u043a\u0442 \u00ab\u0420\u0430\u0437\u0433\u043e\u0432\u043e\u0440\u044b \u043e \u0432\u0430\u0436\u043d\u043e\u043c\u00bb \u043d\u0430 \u0434\u0435\u0442\u0441\u043a\u0438\u0435 \u0441\u0430\u0434\u044b  \u041d\u0430 \u0432\u0441\u0442\u0440\u0435\u0447\u0435 \u0441 \u043b\u0430\u0443\u0440\u0435\u0430\u0442\u0430\u043c\u0438 \u0438 \u0444\u0438\u043d\u0430\u043b\u0438\u0441\u0442\u0430\u043c\u0438 \u043a\u043e\u043d\u043a\u0443\u0440\u0441\u0430 \u00ab\u0423\u0447\u0438\u0442\u0435\u043b\u044c \u0433\u043e\u0434\u0430\u00bb \u041f\u0443\u0442\u0438\u043d \u043f\u043e\u0434\u0434\u0435\u0440\u0436\u0430\u043b \u0438\u0434\u0435\u044e \u0440\u0430\u0441\u043f\u0440\u043e\u0441\u0442\u0440\u0430\u043d\u0438\u0442\u044c \u043f\u0440\u043e\u0435\u043a\u0442 \u00ab\u0420\u0430\u0437\u0433\u043e\u0432\u043e\u0440\u044b \u043e \u0432\u0430\u0436\u043d\u043e\u043c\u00bb \u043d\u0430 \u0434\u0435\u0442\u0441\u043a\u0438\u0435 \u0441\u0430\u0434\u044b. \u041f\u043e \u0441\u043b\u043e\u0432\u0430\u043c \u043f\u0440\u0435\u0437\u0438\u0434\u0435\u043d\u0442\u0430, \u0431\u0430\u0437\u043e\u0432\u044b\u0435 \u0446\u0435\u043d\u043d\u043e\u0441\u0442\u0438 \u0441\u0442\u0440\u0430\u043d\u044b \u043d\u0443\u0436\u043d\u043e \u00ab\u0434\u043e\u0441\u0442\u0443\u043f\u043d\u043e \u0438 \u0430\u043a\u043a\u0443\u0440\u0430\u0442\u043d\u043e \u0434\u043e\u0432\u043e\u0434\u0438\u0442\u044c \u0434\u043e \u0441\u0430\u043c\u044b\u0445 \u043c\u0430\u043b\u0435\u043d\u044c\u043a\u0438\u0445 \u0440\u043e\u0441\u0441\u0438\u044f\u043d\u00bb.  \ud83d\udcac\u042d\u0442\u043e \u0441\u0435\u0440\u044c\u0435\u0437\u043d\u043e\u0435 \u0442\u0430\u043a\u043e\u0435, \u043d\u0430\u0447\u0430\u043b\u043e \u0431\u043e\u043b\u044c\u0448\u043e\u0439 \u0440\u0430\u0431\u043e\u0442\u044b. \u0417\u0434\u0435\u0441\u044c \u0432\u0430\u0436\u043d\u043e \u043d\u0435 \u043f\u0435\u0440\u0435\u0433\u0438\u0431\u0430\u0442\u044c \u0442\u043e\u043b\u044c\u043a\u043e \u043d\u0438\u0447\u0435\u0433\u043e, \u043f\u043e\u043d\u0438\u043c\u0430\u0435\u0442\u0435? \u0412\u0441\u0435 \u0434\u043e\u043b\u0436\u043d\u043e \u0431\u044b\u0442\u044c \u0432 \u043c\u0435\u0440\u0443. \u042d\u0442\u043e \u043f\u0435\u0440\u0432\u043e\u0435. \u0412\u0442\u043e\u0440\u043e\u0435 \u2014 \u0432\u0441\u0435 \u0434\u043e\u043b\u0436\u043d\u043e \u0431\u044b\u0442\u044c \u0438\u0441\u043a\u0440\u0435\u043d\u043d\u0435, \u043e\u0431\u044a\u0435\u043a\u0442\u0438\u0432\u043d\u043e, \u0434\u043e\u0445\u043e\u0434\u0447\u0438\u0432\u043e\ud83d\udcac, \u2014 \u0441\u043a\u0430\u0437\u0430\u043b \u043f\u0440\u0435\u0437\u0438\u0434\u0435\u043d\u0442.\u041f\u0443\u0442\u0438\u043d \u043d\u0430\u043f\u043e\u043c\u043d\u0438\u043b, \u0447\u0442\u043e \u0432 \u0420\u043e\u0441\u0441\u0438\u0438 \u0435\u0441\u0442\u044c \u0442\u0430\u043a\u0438\u0435 \u0432\u044b\u0440\u0430\u0436\u0435\u043d\u0438\u044f, \u043a\u0430\u043a \u00ab\u0432\u043f\u0438\u0442\u0430\u043b \u0441 \u043c\u043e\u043b\u043e\u043a\u043e\u043c \u043c\u0430\u0442\u0435\u0440\u0438\u00bb \u0438\u043b\u0438 \u00ab\u0443\u0441\u0432\u043e\u0438\u043b \u0441 \u043c\u043b\u0430\u0434\u044b\u0445 \u043d\u043e\u0433\u0442\u0435\u0439\u00bb. \u0422\u0430\u043a\u0436\u0435 \u043f\u0440\u0435\u0437\u0438\u0434\u0435\u043d\u0442 \u043f\u043e\u0434\u0447\u0435\u0440\u043a\u043d\u0443\u043b \u043d\u0435\u043e\u0431\u0445\u043e\u0434\u0438\u043c\u043e\u0441\u0442\u044c \u0432\u043e\u0441\u043f\u0438\u0442\u0430\u043d\u0438\u044f \u0432 \u0434\u0435\u0442\u044f\u0445 \u043a\u0443\u043b\u044c\u0442\u0443\u0440\u044b \u0440\u0435\u0447\u0438 \u0438 \u043b\u044e\u0431\u0432\u0438 \u043a \u0447\u0442\u0435\u043d\u0438\u044e, \u043e\u0442\u043c\u0435\u0442\u0438\u0432, \u0447\u0442\u043e \u0432 \u0441\u043e\u0432\u0440\u0435\u043c\u0435\u043d\u043d\u043e\u043c \u043c\u0438\u0440\u0435 \u043d\u0435 \u0442\u043e\u043b\u044c\u043a\u043e \u00ab\u043f\u0430\u043b\u044c\u0447\u0438\u043a\u043e\u043c \u043a\u043d\u043e\u043f\u043e\u0447\u043a\u0438 \u043d\u0430\u0436\u0438\u043c\u0430\u0442\u044c \u0432\u0430\u0436\u043d\u043e\u00bb", "4": "<b>Total Posts:</b> 89<br><b>Date:</b> 2024-10-03 13:28:59+00:00<br><b>Author:</b> mod_russia<br><b>Link:</b> https://t.me/s/mod_russia/44084<br><b>Subscribers:</b> 602674<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \ud83d\udd25 \u0423\u043d\u0438\u0447\u0442\u043e\u0436\u0435\u043d\u0438\u0435 \u0431\u043e\u0435\u0432\u043e\u0439 \u043c\u0430\u0448\u0438\u043d\u044b \u0417\u0420\u041f\u041a \u00ab\u0422\u0443\u043d\u0433\u0443\u0441\u043a\u0430\u00bb \u0412\u0421\u0423 \u0431\u0430\u0440\u0440\u0430\u0436\u0438\u0440\u0443\u044e\u0449\u0438\u043c \u0431\u043e\u0435\u043f\u0440\u0438\u043f\u0430\u0441\u043e\u043c \u00ab\u041b\u0430\u043d\u0446\u0435\u0442\u00bb \u0432 \u043f\u0440\u0438\u0433\u0440\u0430\u043d\u0438\u0447\u043d\u043e\u043c \u0440\u0430\u0439\u043e\u043d\u0435 \u041a\u0443\u0440\u0441\u043a\u043e\u0439 \u043e\u0431\u043b\u0430\u0441\u0442\u0438  \ud83d\udd39 \u041c\u0438\u043d\u043e\u0431\u043e\u0440\u043e\u043d\u044b \u0420\u043e\u0441\u0441\u0438\u0438", "5": "<b>Total Posts:</b> 16<br><b>Date:</b> 2024-10-03 07:35:43+00:00<br><b>Author:</b> russianonwars<br><b>Link:</b> https://t.me/s/russianonwars/36406<br><b>Subscribers:</b> 379147<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u041f\u0440\u0435\u0434\u0441\u0435\u0434\u0430\u0442\u0435\u043b\u044c \u043f\u0430\u0440\u043b\u0430\u043c\u0435\u043d\u0442\u0430 \u0413\u0440\u0443\u0437\u0438\u0438 \u043f\u043e\u0434\u043f\u0438\u0441\u0430\u043b \u0437\u0430\u043a\u043e\u043d \u043e \u0437\u0430\u043f\u0440\u0435\u0442\u0435 \u0432 \u0441\u0442\u0440\u0430\u043d\u0435 \u041b\u0413\u0411\u0422*-\u043f\u0440\u043e\u043f\u0430\u0433\u0430\u043d\u0434\u044b\u041f\u0430\u0440\u043b\u0430\u043c\u0435\u043d\u0442 \u0441\u0442\u0440\u0430\u043d\u044b \u043f\u0440\u0438\u043d\u044f\u043b \u0435\u0433\u043e, \u043d\u043e \u0433\u0440\u0443\u0437\u0438\u043d\u0441\u043a\u0438\u0439 \u043f\u0440\u0435\u0437\u0438\u0434\u0435\u043d\u0442 \u043e\u0442\u043a\u0430\u0437\u0430\u043b\u0441\u044f \u0435\u0433\u043e \u043f\u043e\u0434\u043f\u0438\u0441\u0430\u0442\u044c, \u0447\u0442\u043e \u0432\u043f\u0440\u043e\u0447\u0435\u043c \u043d\u0435 \u043f\u043e\u043c\u0435\u0448\u0430\u043b\u043e \u0435\u0433\u043e \u0432\u0441\u0442\u0443\u043f\u043b\u0435\u043d\u0438\u044e \u0432 \u0434\u0435\u0439\u0441\u0442\u0432\u0438\u0435. \u0421\u043e\u0433\u043b\u0430\u0441\u043d\u043e \u0437\u0430\u043a\u043e\u043d\u0430\u043c \u043a\u0430\u0432\u043a\u0430\u0437\u0441\u043a\u043e\u0439 \u0441\u0442\u0440\u0430\u043d\u044b, \u0432 \u0441\u043b\u0443\u0447\u0430\u0435 \u043e\u0442\u043a\u0430\u0437\u0430 \u0433\u043b\u0430\u0432\u044b \u0433\u043e\u0441\u0443\u0434\u0430\u0440\u0441\u0442\u0432\u0430 \u043f\u043e\u0434\u043f\u0438\u0441\u0430\u0442\u044c \u0437\u0430\u043a\u043e\u043d \u0437\u0430 \u043d\u0435\u0433\u043e \u044d\u0442\u043e \u043c\u043e\u0436\u0435\u0442 \u0441\u0434\u0435\u043b\u0430\u0442\u044c \u0441\u043f\u0438\u043a\u0435\u0440 \u043f\u0430\u0440\u043b\u0430\u043c\u0435\u043d\u0442\u0430, \u0447\u0442\u043e \u0438 \u043f\u0440\u043e\u0438\u0437\u043e\u0448\u043b\u043e.\u0415\u0421 \u0433\u0440\u043e\u0437\u0438\u043b\u0441\u044f \u043e\u0442\u043c\u0435\u043d\u0438\u0442\u044c \u0431\u0435\u0437\u0432\u0438\u0437 \u0434\u043b\u044f \u0413\u0440\u0443\u0437\u0438\u0438 \u0432 \u0441\u043b\u0443\u0447\u0430\u0435 \u043f\u0440\u0438\u043d\u044f\u0442\u0438\u044f \u044d\u0442\u043e\u0433\u043e \u0437\u0430\u043a\u043e\u043d\u0430. \u0415\u0432\u0440\u043e\u0438\u043d\u0442\u0435\u0433\u0440\u0430\u0446\u0438\u044f \u0441\u0442\u0440\u0430\u043d\u044b \u0431\u044b\u043b\u0430 \u043f\u0440\u0438\u043e\u0441\u0442\u0430\u043d\u043e\u0432\u043b\u0435\u043d\u0430 \u043f\u043e\u0441\u043b\u0435 \u043f\u0440\u0438\u043d\u044f\u0442\u0438\u044f \u0437\u0430\u043a\u043e\u043d\u0430 \u043e\u0431 \u0438\u043d\u043e\u0430\u0433\u0435\u043d\u0442\u0430\u0445.* \u2014 \u0437\u0430\u043f\u0440\u0435\u0449\u0435\u043d\u043d\u0430\u044f \u0432 \u0420\u043e\u0441\u0441\u0438\u0438 \u044d\u043a\u0441\u0442\u0440\u0435\u043c\u0438\u0441\u0442\u0441\u043a\u0430\u044f \u043e\u0440\u0433\u0430\u043d\u0438\u0437\u0430\u0446\u0438\u044f\u2764\ufe0f \u041f\u043e\u0434\u043f\u0438\u0441\u044b\u0432\u0430\u0439\u0441\u044f \u043d\u0430 \"\u0413\u043e\u043b\u043e\u0441 \u0441\u0442\u0440\u0430\u043d\u044b\"", "6": "<b>Total Posts:</b> 120<br><b>Date:</b> 2024-10-03 19:23:55+00:00<br><b>Author:</b> radarrussiia<br><b>Link:</b> https://t.me/s/radarrussiia/12552<br><b>Subscribers:</b> 408472<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u0412\u043e\u0440\u043e\u043d\u0435\u0436\u0441\u043a\u0430\u044f \u043e\u0431\u043b\u0430\u0441\u0442\u044c - \u043e\u043f\u0430\u0441\u043d\u043e\u0441\u0442\u044c \u0411\u041f\u041b\u0410.\u2757\ufe0f\u0420\u0430\u0434\u0430\u0440 \u043f\u043e \u0432\u0441\u0435\u0439 \u0420\u043e\u0441\u0441\u0438\u0438 - @radarrussiia", "7": "<b>Total Posts:</b> 18<br><b>Date:</b> 2024-10-03 06:56:20+00:00<br><b>Author:</b> treugolniklpr<br><b>Link:</b> https://t.me/s/treugolniklpr/62112<br><b>Subscribers:</b> 642721<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u0413\u043e\u0440\u043b\u043e\u0432\u043a\u0430\u0410\u0440\u0442\u0435\u043c\u043e\u0432\u0441\u043a \u0414\u043e\u043d\u0435\u0446\u043a \u0423\u0433\u043b\u0435\u0434\u0430\u0440 \u0421\u0435\u043b\u0438\u0434\u043e\u0432\u043e \u0412\u043e\u043b\u043d\u043e\u0432\u0430\u0445\u0430 \u0418 \u0431\u043b\u0438\u0437\u043b\u0435\u0436\u0430\u0449\u0438\u0435 \u0410\u0432\u0438\u0430\u0446\u0438\u043e\u043d\u043d\u0430\u044f \u0440\u0430\u043a\u0435\u0442\u043d\u0430\u044f \u0431\u043e\u043c\u0431\u043e\u0432\u0430\u044f \u043e\u043f\u0430\u0441\u043d\u043e\u0441\u0442\u044c \u041a 10-10", "8": "<b>Total Posts:</b> 13<br><b>Date:</b> 2024-10-03 04:17:10+00:00<br><b>Author:</b> rt_russian<br><b>Link:</b> https://t.me/s/rt_russian/217081<br><b>Subscribers:</b> 992621<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u0421\u0438\u043b\u044b \u041f\u0412\u041e \u043f\u0435\u0440\u0435\u0445\u0432\u0430\u0442\u0438\u043b\u0438 \u0438 \u0443\u043d\u0438\u0447\u0442\u043e\u0436\u0438\u043b\u0438 \u0437\u0430 \u043d\u043e\u0447\u044c 113 \u0443\u043a\u0440\u0430\u0438\u043d\u0441\u043a\u0438\u0445 \u0411\u041f\u041b\u0410 \u2014 \u041c\u0438\u043d\u043e\u0431\u043e\u0440\u043e\u043d\u044b \u0420\u0424.73 \u0431\u0435\u0441\u043f\u0438\u043b\u043e\u0442\u043d\u0438\u043a\u0430 \u043f\u043e\u0440\u0430\u0436\u0435\u043d\u044b \u043d\u0430\u0434 \u0411\u0435\u043b\u0433\u043e\u0440\u043e\u0434\u0441\u043a\u043e\u0439 \u043e\u0431\u043b\u0430\u0441\u0442\u044c\u044e, 25 \u2014 \u043d\u0430\u0434 \u0412\u043e\u0440\u043e\u043d\u0435\u0436\u0441\u043a\u043e\u0439, 14 \u2014 \u043d\u0430\u0434 \u041a\u0443\u0440\u0441\u043a\u043e\u0439 \u0438 \u043e\u0434\u0438\u043d \u2014 \u043d\u0430\u0434 \u0411\u0440\u044f\u043d\u0441\u043a\u043e\u0439.\ud83d\udfe9 \u041f\u043e\u0434\u043f\u0438\u0441\u0430\u0442\u044c\u0441\u044f | \u041f\u0440\u0438\u0441\u043b\u0430\u0442\u044c \u043d\u043e\u0432\u043e\u0441\u0442\u044c | \u0417\u0435\u0440\u043a\u0430\u043b\u043e"};

    function displayClusterText() {
        var selectedLabel = document.getElementById("clusterSelector").value;
        var details = clusterDetails[selectedLabel];
        var textDiv = document.getElementById("clusterTextDisplay");
        textDiv.innerHTML = '<p>' + details + '</p>';
        textDiv.classList.remove('hidden');
    }
</script>
