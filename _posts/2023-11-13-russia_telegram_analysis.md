---
layout: post
title: "Russia Telegram Analysis - 2023-11-13"
author: "Dmytro Bukhanevych"
categories: analysis
tags: [telegram, analysis]
image: pawel-czerwinski-fRzUPSFnp04-unsplash.jpg
permalink: "/analysis/russia-telegram-analysis-2023-11-13"
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
<p>Загалом було проаналізовано 5845 постів у Telegram за період з 10.11.2023 до 12.11.2023. Було відстежено активність 121 найбільш популярних Telegram каналів у Росії. Після попередньої обробки, фільтрування за ключовими словами, кластеризації та зменшення шуму, 838 текстів було проаналізовано у крайньому звітному періоді.</p>
<!-- Embedding Main Plotly Visualization -->
<div class="wide-iframe-container">
    <iframe src="{{site.baseurl}}/visualizations/2023-11-13/fig_topics_time.html" height="850"></iframe>
</div>


<h2>Cluster Text</h2>

<!-- Dropdown to select a cluster -->
<select id="clusterSelector" onchange="displayClusterText()">
<option value="0">Cluster 0</option><option value="1">Cluster 1</option><option value="2">Cluster 2</option><option value="3">Cluster 3</option><option value="4">Cluster 4</option><option value="5">Cluster 5</option><option value="6">Cluster 6</option><option value="7">Cluster 7</option><option value="8">Cluster 8</option><option value="9">Cluster 9</option>
</select>

<!-- Display area for the selected cluster's text -->
<div id="clusterTextDisplay" class="hidden"></div>

<script type="text/javascript">
    var clusterDetails = {"0": "<b>Total Posts:</b> 81<br><b>Date:</b> 2023-11-12 09:50:43+00:00<br><b>Author:</b> bbbreaking<br><b>Link:</b> https://t.me/s/bbbreaking/169456<br><b>Subscribers:</b> 1555810<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u041f\u0435\u0441\u043a\u043e\u0432: \u0423\u043a\u0440\u0430\u0438\u043d\u0435 \u043d\u0443\u0436\u043d\u043e \u043f\u043e\u043d\u044f\u0442\u044c, \u0447\u0442\u043e \u043f\u043e\u0431\u0435\u0434\u0438\u0442\u044c \u0420\u0424 \u043d\u0435\u0432\u043e\u0437\u043c\u043e\u0436\u043d\u043e", "1": "<b>Total Posts:</b> 219<br><b>Date:</b> 2023-11-12 11:33:55+00:00<br><b>Author:</b> boris_rozhin<br><b>Link:</b> https://t.me/s/boris_rozhin/103640<br><b>Subscribers:</b> 806001<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u0421\u0432\u043e\u0434\u043a\u0430 \u041c\u0438\u043d\u0438\u0441\u0442\u0435\u0440\u0441\u0442\u0432\u0430 \u043e\u0431\u043e\u0440\u043e\u043d\u044b \u0420\u043e\u0441\u0441\u0438\u0439\u0441\u043a\u043e\u0439 \u0424\u0435\u0434\u0435\u0440\u0430\u0446\u0438\u0438 \u043e \u0445\u043e\u0434\u0435 \u043f\u0440\u043e\u0432\u0435\u0434\u0435\u043d\u0438\u044f \u0441\u043f\u0435\u0446\u0438\u0430\u043b\u044c\u043d\u043e\u0439 \u0432\u043e\u0435\u043d\u043d\u043e\u0439 \u043e\u043f\u0435\u0440\u0430\u0446\u0438\u0438 (\u043f\u043e \u0441\u043e\u0441\u0442\u043e\u044f\u043d\u0438\u044e \u043d\u0430 12 \u043d\u043e\u044f\u0431\u0440\u044f 2023 \u0433.) \u0413\u043b\u0430\u0432\u043d\u043e\u0435:\u0412\u0421 \u0420\u0424 \u043d\u0430 \u043a\u0443\u043f\u044f\u043d\u0441\u043a\u043e\u043c \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438 \u043e\u0442\u0440\u0430\u0437\u0438\u043b\u0438 \u0434\u0432\u0435 \u0430\u0442\u0430\u043a\u0438, \u0430 \u0442\u0430\u043a\u0436\u0435 \u0443\u043d\u0438\u0447\u0442\u043e\u0436\u0438\u043b\u0438 \u0441\u043a\u043b\u0430\u0434 \u0431\u043e\u0435\u043f\u0440\u0438\u043f\u0430\u0441\u043e\u0432 \u0443\u043a\u0440\u0430\u0438\u043d\u0441\u043a\u043e\u0439 \u0442\u0435\u0440\u043e\u0431\u043e\u0440\u043e\u043d\u044b;\u2014\u0412 \u0440\u0430\u0439\u043e\u043d\u0435 \u0420\u0430\u0431\u043e\u0442\u0438\u043d\u0430 \u043d\u0430\u043d\u0435\u0441\u0435\u043d\u043e \u043e\u0433\u043d\u0435\u0432\u043e\u0435 \u043f\u043e\u0440\u0430\u0436\u0435\u043d\u0438\u0435 \u0441\u043a\u043e\u043f\u043b\u0435\u043d\u0438\u044f\u043c \u0436\u0438\u0432\u043e\u0439 \u0441\u0438\u043b\u044b \u0438 \u0442\u0435\u0445\u043d\u0438\u043a\u0438 33-\u0439 \u043c\u0435\u0445\u0430\u043d\u0438\u0437\u0438\u0440\u043e\u0432\u0430\u043d\u043d\u043e\u0439 \u0431\u0440\u0438\u0433\u0430\u0434\u044b \u0412\u0421\u0423;\u2014\u0412\u0421\u0423 \u043d\u0430 \u0434\u043e\u043d\u0435\u0446\u043a\u043e\u043c \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438 \u043f\u043e\u0442\u0435\u0440\u044f\u043b\u0438 \u0434\u043e 250 \u0432\u043e\u0435\u043d\u043d\u044b\u0445 \u0443\u0431\u0438\u0442\u044b\u043c\u0438 \u0438 \u0440\u0430\u043d\u0435\u043d\u044b\u043c\u0438, \u0430 \u0442\u0430\u043a\u0436\u0435 \u0442\u0440\u0438 \u0431\u0440\u043e\u043d\u0435\u043c\u0430\u0448\u0438\u043d\u044b \u0438 \u0442\u0440\u0438 \u043f\u0438\u043a\u0430\u043f\u0430;\u2014\u041f\u043e\u0442\u0435\u0440\u0438 \u0412\u0421\u0423 \u0437\u0430 \u0441\u0443\u0442\u043a\u0438 \u043d\u0430 \u0445\u0435\u0440\u0441\u043e\u043d\u0441\u043a\u043e\u043c \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438 \u0441\u043e\u0441\u0442\u0430\u0432\u0438\u043b\u0438 \u0434\u043e 60 \u0447\u0435\u043b\u043e\u0432\u0435\u043a;\u2014\u0412\u0421 \u0420\u0424 \u043f\u043e\u0440\u0430\u0437\u0438\u043b\u0438 \u043f\u0443\u043d\u043a\u0442 \u0443\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u044f \u0431\u0440\u0438\u0433\u0430\u0434\u044b \u0412\u0421\u0423 \u0443 \u0410\u043d\u0442\u043e\u043d\u043e\u0432\u043a\u0438 \u0432 \u0414\u041d\u0420 \u0438 \u0443\u043d\u0438\u0447\u0442\u043e\u0436\u0438\u043b\u0438 \u0441\u043a\u043b\u0430\u0434 \u0433\u043e\u0440\u044e\u0447\u0435\u0433\u043e \u0443 \u041a\u043e\u043d\u0441\u0442\u0430\u043d\u0442\u0438\u043d\u043e\u0432\u043a\u0438 \u0432 \u041d\u0438\u043a\u043e\u043b\u0430\u0435\u0432\u0441\u043a\u043e\u0439 \u043e\u0431\u043b\u0430\u0441\u0442\u0438;\u2014\u0412\u0421 \u0420\u0424 \u043e\u0442\u0440\u0430\u0437\u0438\u043b\u0438 \u0437\u0430 \u0441\u0443\u0442\u043a\u0438 2 \u0430\u0442\u0430\u043a\u0438 \u0412\u0421\u0423 \u043d\u0430 \u043a\u0440\u0430\u0441\u043d\u043e\u043b\u0438\u043c\u0430\u043d\u0441\u043a\u043e\u043c \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438, \u043f\u043e\u0442\u0435\u0440\u0438 \u043f\u0440\u043e\u0442\u0438\u0432\u043d\u0438\u043a\u0430 \u0441\u043e\u0441\u0442\u0430\u0432\u0438\u043b\u0438 \u0434\u043e 210 \u0432\u043e\u0435\u043d\u043d\u043e\u0441\u043b\u0443\u0436\u0430\u0449\u0438\u0445. \u2014\u0417\u0430 \u0441\u0443\u0442\u043a\u0438 \u0441\u0440\u0435\u0434\u0441\u0442\u0432\u0430 \u041f\u0412\u041e \u0420\u0424 \u043f\u0435\u0440\u0435\u0445\u0432\u0430\u0442\u0438\u043b\u0438 \u0434\u0432\u0430 \u0441\u043d\u0430\u0440\u044f\u0434\u0430 \u0420\u0421\u0417\u041e HIMARS \u0438 \u0441\u0431\u0438\u043b\u0438 42 \u0431\u0435\u0441\u043f\u0438\u043b\u043e\u0442\u043d\u0438\u043a\u0430 \u0412\u0421\u0423;\u2014\u041f\u043e\u0442\u0435\u0440\u0438 \u0412\u0421\u0423 \u043d\u0430 \u044e\u0436\u043d\u043e\u0434\u043e\u043d\u0435\u0446\u043a\u043e\u043c \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438 \u0437\u0430 \u0441\u0443\u0442\u043a\u0438 \u0441\u043e\u0441\u0442\u0430\u0432\u0438\u043b\u0438 \u0441\u0432\u044b\u0448\u0435 80 \u0432\u043e\u0435\u043d\u043d\u043e\u0441\u043b\u0443\u0436\u0430\u0449\u0438\u0445.\u0412\u0441\u0435\u0433\u043e \u0441 \u043d\u0430\u0447\u0430\u043b\u0430 \u043f\u0440\u043e\u0432\u0435\u0434\u0435\u043d\u0438\u044f \u0441\u043f\u0435\u0446\u0438\u0430\u043b\u044c\u043d\u043e\u0439 \u0432\u043e\u0435\u043d\u043d\u043e\u0439 \u043e\u043f\u0435\u0440\u0430\u0446\u0438\u0438 \u0443\u043d\u0438\u0447\u0442\u043e\u0436\u0435\u043d\u043e: 534 \u0441\u0430\u043c\u043e\u043b\u0435\u0442\u0430, 254 \u0432\u0435\u0440\u0442\u043e\u043b\u0435\u0442\u0430, 8871 \u0431\u0435\u0441\u043f\u0438\u043b\u043e\u0442\u043d\u044b\u0439 \u043b\u0435\u0442\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439 \u0430\u043f\u043f\u0430\u0440\u0430\u0442, 441 \u0437\u0435\u043d\u0438\u0442\u043d\u044b\u0439 \u0440\u0430\u043a\u0435\u0442\u043d\u044b\u0439 \u043a\u043e\u043c\u043f\u043b\u0435\u043a\u0441, 13358 \u0442\u0430\u043d\u043a\u043e\u0432 \u0438 \u0434\u0440\u0443\u0433\u0438\u0445 \u0431\u043e\u0435\u0432\u044b\u0445 \u0431\u0440\u043e\u043d\u0438\u0440\u043e\u0432\u0430\u043d\u043d\u044b\u0445 \u043c\u0430\u0448\u0438\u043d, 1183 \u0431\u043e\u0435\u0432\u044b\u0435 \u043c\u0430\u0448\u0438\u043d\u044b \u0440\u0435\u0430\u043a\u0442\u0438\u0432\u043d\u044b\u0445 \u0441\u0438\u0441\u0442\u0435\u043c \u0437\u0430\u043b\u043f\u043e\u0432\u043e\u0433\u043e \u043e\u0433\u043d\u044f, 7071 \u043e\u0440\u0443\u0434\u0438\u0435 \u043f\u043e\u043b\u0435\u0432\u043e\u0439 \u0430\u0440\u0442\u0438\u043b\u043b\u0435\u0440\u0438\u0438 \u0438 \u043c\u0438\u043d\u043e\u043c\u0435\u0442\u043e\u0432, \u0430 \u0442\u0430\u043a\u0436\u0435 15207 \u0435\u0434\u0438\u043d\u0438\u0446 \u0441\u043f\u0435\u0446\u0438\u0430\u043b\u044c\u043d\u043e\u0439 \u0432\u043e\u0435\u043d\u043d\u043e\u0439 \u0430\u0432\u0442\u043e\u043c\u043e\u0431\u0438\u043b\u044c\u043d\u043e\u0439 \u0442\u0435\u0445\u043d\u0438\u043a\u0438.\u0427\u0438\u0442\u0430\u0442\u044c \u043f\u043e\u043b\u043d\u043e\u0441\u0442\u044c\u044e: |\u0447\u0430\u0441\u0442\u044c1 |\u0447\u0430\u0441\u0442\u044c2 |", "2": "<b>Total Posts:</b> 29<br><b>Date:</b> 2023-11-12 12:10:01+00:00<br><b>Author:</b> rt_russian<br><b>Link:</b> https://t.me/s/rt_russian/179711<br><b>Subscribers:</b> 797053<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u0410\u0440\u043c\u0438\u044f \u0418\u0437\u0440\u0430\u0438\u043b\u044f \u043f\u043e\u043a\u0430\u0437\u0430\u043b\u0430 \u043a\u0430\u0434\u0440\u044b \u0430\u0442\u0430\u043a\u0438 \u043f\u043e \u0440\u0430\u043a\u0435\u0442\u0447\u0438\u043a\u0430\u043c \u0432 \u0436\u0438\u043b\u043e\u043c \u0440\u0430\u0439\u043e\u043d\u0435 \u041b\u0438\u0432\u0430\u043d\u0430, \u043a\u043e\u0442\u043e\u0440\u044b\u0435 \u0445\u043e\u0442\u0435\u043b\u0438 \u0432\u0435\u0441\u0442\u0438 \u043e\u0433\u043e\u043d\u044c \u043f\u043e \u0438\u0437\u0440\u0430\u0438\u043b\u044c\u0441\u043a\u043e\u0439 \u0442\u0435\u0440\u0440\u0438\u0442\u043e\u0440\u0438\u0438. \u0412 \u0426\u0410\u0425\u0410\u041b \u0442\u0430\u043a\u0436\u0435 \u0437\u0430\u044f\u0432\u0438\u043b\u0438, \u0447\u0442\u043e \u043e\u0442\u0440\u0430\u0431\u0430\u0442\u044b\u0432\u0430\u044e\u0442 \u043f\u043e \u043c\u0435\u0441\u0442\u0443 \u0437\u0430\u043f\u0443\u0441\u043a\u0430 \u041f\u0422\u0420\u041a \u0432 \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438 \u0414\u043e\u0432\u0435\u0432\u0430 \u043d\u0430 \u0442\u0435\u0440\u0440\u0438\u0442\u043e\u0440\u0438\u0438 \u0418\u0437\u0440\u0430\u0438\u043b\u044f.\ud83d\udfe9 RT \u043d\u0430 \u0440\u0443\u0441\u0441\u043a\u043e\u043c. \u041f\u043e\u0434\u043f\u0438\u0448\u0438\u0441\u044c", "3": "<b>Total Posts:</b> 20<br><b>Date:</b> 2023-11-12 18:02:06+00:00<br><b>Author:</b> dmitrynikotin<br><b>Link:</b> https://t.me/s/dmitrynikotin/14966<br><b>Subscribers:</b> 648517<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \ud83c\uddfa\ud83c\uddf8\u0420\u0430\u0437\u0431\u0438\u043b\u0441\u044f \u0430\u043c\u0435\u0440\u0438\u043a\u0430\u043d\u0441\u043a\u0438\u0439 \u0432\u043e\u0435\u043d\u043d\u044b\u0439 \u0441\u0430\u043c\u043e\u043b\u0435\u0442.\u041f\u044f\u0442\u044c \u0430\u043c\u0435\u0440\u0438\u043a\u0430\u043d\u0441\u043a\u0438\u0445 \u0432\u043e\u0435\u043d\u043d\u044b\u0445 \u043f\u043e\u0433\u0438\u0431\u043b\u0438 \u0432 \u043a\u0430\u0442\u0430\u0441\u0442\u0440\u043e\u0444\u0435 \u0441\u0430\u043c\u043e\u043b\u0435\u0442\u0430 \u043f\u0440\u0438 \u0434\u043e\u0437\u0430\u043f\u0440\u0430\u0432\u043a\u0435 \u043d\u0430\u0434 \u0421\u0440\u0435\u0434\u0438\u0437\u0435\u043c\u043d\u044b\u043c \u043c\u043e\u0440\u0435\u043c, \u0441\u043e\u043e\u0431\u0449\u0438\u043b\u043e \u0415\u0432\u0440\u043e\u043f\u0435\u0439\u0441\u043a\u043e\u0435 \u043a\u043e\u043c\u0430\u043d\u0434\u043e\u0432\u0430\u043d\u0438\u0435 \u041f\u0435\u043d\u0442\u0430\u0433\u043e\u043d\u0430.", "4": "<b>Total Posts:</b> 13<br><b>Date:</b> 2023-11-12 15:11:02+00:00<br><b>Author:</b> swodki<br><b>Link:</b> https://t.me/s/swodki/320780<br><b>Subscribers:</b> 257477<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \ud83c\uddf7\ud83c\uddfa\ud83d\udca5\u0411\u043e\u0438 \u0443 \u041a\u043b\u0435\u0449\u0435\u0435\u0432\u043a\u0438: \u0443\u043d\u0438\u0447\u0442\u043e\u0436\u0435\u043d\u0438\u0435 \u041f\u0422\u0423\u0420\u043e\u043c \u0433\u0440\u0443\u043f\u043f\u044b \u0431\u043e\u0435\u0432\u0438\u043a\u043e\u0432\u0411\u043e\u0439\u0446\u044b \u00ab\u042e\u0436\u043d\u043e\u0439\u00bb \u0433\u0440\u0443\u043f\u043f\u0438\u0440\u043e\u0432\u043a\u0438 \u0442\u043e\u0447\u043d\u044b\u043c \u043f\u043e\u043f\u0430\u0434\u0430\u043d\u0438\u0435\u043c \u0438\u0437 \u041f\u0422\u0420\u041a \u0443\u043d\u0438\u0447\u0442\u043e\u0436\u0438\u043b\u0438 \u0433\u0440\u0443\u043f\u043f\u0443 \u0431\u043e\u0435\u0432\u0438\u043a\u043e\u0432 \u0438\u0437 22 \u043e\u0442\u0434\u0435\u043b\u044c\u043d\u043e\u0439 \u043c\u0435\u0445\u0431\u0440\u0438\u0433\u0430\u0434\u044b \u0412\u0421\u0423 \u043d\u0430 \u0410\u0440\u0442\u0435\u043c\u043e\u0432\u0441\u043a\u043e\u043c \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438.", "5": "<b>Total Posts:</b> 37<br><b>Date:</b> 2023-11-12 11:29:19+00:00<br><b>Author:</b> solovievlive<br><b>Link:</b> https://t.me/s/SolovievLive/221101<br><b>Subscribers:</b> 1299944<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u2757\ufe0f\u0413\u043b\u0430\u0432\u043d\u043e\u0435 \u0438\u0437 \u043d\u043e\u0432\u043e\u0433\u043e \u0431\u0440\u0438\u0444\u0438\u043d\u0433\u0430 \u041c\u0438\u043d\u043e\u0431\u043e\u0440\u043e\u043d\u044b \u0420\u043e\u0441\u0441\u0438\u0438:\ud83d\udccc\u0412\u0421 \u0420\u0424 \u043d\u0430 \u043a\u0443\u043f\u044f\u043d\u0441\u043a\u043e\u043c \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438 \u043e\u0442\u0440\u0430\u0437\u0438\u043b\u0438 \u0434\u0432\u0435 \u0430\u0442\u0430\u043a\u0438, \u0430 \u0442\u0430\u043a\u0436\u0435 \u0443\u043d\u0438\u0447\u0442\u043e\u0436\u0438\u043b\u0438 \u0441\u043a\u043b\u0430\u0434 \u0431\u043e\u0435\u043f\u0440\u0438\u043f\u0430\u0441\u043e\u0432 \u0443\u043a\u0440\u0430\u0438\u043d\u0441\u043a\u043e\u0439 \u0442\u0435\u0440\u043e\u0431\u043e\u0440\u043e\u043d\u044b;\ud83d\udccc\u0412 \u0440\u0430\u0439\u043e\u043d\u0435 \u0420\u0430\u0431\u043e\u0442\u0438\u043d\u0430 \u043d\u0430\u043d\u0435\u0441\u0435\u043d\u043e \u043e\u0433\u043d\u0435\u0432\u043e\u0435 \u043f\u043e\u0440\u0430\u0436\u0435\u043d\u0438\u0435 \u0441\u043a\u043e\u043f\u043b\u0435\u043d\u0438\u044f\u043c \u0436\u0438\u0432\u043e\u0439 \u0441\u0438\u043b\u044b \u0438 \u0442\u0435\u0445\u043d\u0438\u043a\u0438 33-\u0439 \u043c\u0435\u0445\u0430\u043d\u0438\u0437\u0438\u0440\u043e\u0432\u0430\u043d\u043d\u043e\u0439 \u0431\u0440\u0438\u0433\u0430\u0434\u044b \u0412\u0421\u0423;\ud83d\udccc\u0412\u0421\u0423 \u043d\u0430 \u0434\u043e\u043d\u0435\u0446\u043a\u043e\u043c \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438 \u043f\u043e\u0442\u0435\u0440\u044f\u043b\u0438 \u0434\u043e 250 \u0432\u043e\u0435\u043d\u043d\u044b\u0445 \u0443\u0431\u0438\u0442\u044b\u043c\u0438 \u0438 \u0440\u0430\u043d\u0435\u043d\u044b\u043c\u0438, \u0430 \u0442\u0430\u043a\u0436\u0435 \u0442\u0440\u0438 \u0431\u0440\u043e\u043d\u0435\u043c\u0430\u0448\u0438\u043d\u044b \u0438 \u0442\u0440\u0438 \u043f\u0438\u043a\u0430\u043f\u0430;\ud83d\udccc\u041f\u043e\u0442\u0435\u0440\u0438 \u0412\u0421\u0423 \u0437\u0430 \u0441\u0443\u0442\u043a\u0438 \u043d\u0430 \u0445\u0435\u0440\u0441\u043e\u043d\u0441\u043a\u043e\u043c \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438 \u0441\u043e\u0441\u0442\u0430\u0432\u0438\u043b\u0438 \u0434\u043e 60 \u0447\u0435\u043b\u043e\u0432\u0435\u043a;\ud83d\udccc\u0412\u0421 \u0420\u0424 \u043f\u043e\u0440\u0430\u0437\u0438\u043b\u0438 \u043f\u0443\u043d\u043a\u0442 \u0443\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u044f \u0431\u0440\u0438\u0433\u0430\u0434\u044b \u0412\u0421\u0423 \u0443 \u0410\u043d\u0442\u043e\u043d\u043e\u0432\u043a\u0438 \u0432 \u0414\u041d\u0420 \u0438 \u0443\u043d\u0438\u0447\u0442\u043e\u0436\u0438\u043b\u0438 \u0441\u043a\u043b\u0430\u0434 \u0433\u043e\u0440\u044e\u0447\u0435\u0433\u043e \u0443 \u041a\u043e\u043d\u0441\u0442\u0430\u043d\u0442\u0438\u043d\u043e\u0432\u043a\u0438 \u0432 \u041d\u0438\u043a\u043e\u043b\u0430\u0435\u0432\u0441\u043a\u043e\u0439 \u043e\u0431\u043b\u0430\u0441\u0442\u0438;\ud83d\udccc\u0412\u0421 \u0420\u0424 \u043e\u0442\u0440\u0430\u0437\u0438\u043b\u0438 \u0437\u0430 \u0441\u0443\u0442\u043a\u0438 2 \u0430\u0442\u0430\u043a\u0438 \u0412\u0421\u0423 \u043d\u0430 \u043a\u0440\u0430\u0441\u043d\u043e\u043b\u0438\u043c\u0430\u043d\u0441\u043a\u043e\u043c \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438, \u043f\u043e\u0442\u0435\u0440\u0438 \u043f\u0440\u043e\u0442\u0438\u0432\u043d\u0438\u043a\u0430 \u0441\u043e\u0441\u0442\u0430\u0432\u0438\u043b\u0438 \u0434\u043e 210 \u0432\u043e\u0435\u043d\u043d\u043e\u0441\u043b\u0443\u0436\u0430\u0449\u0438\u0445. \ud83d\udccc\u0417\u0430 \u0441\u0443\u0442\u043a\u0438 \u0441\u0440\u0435\u0434\u0441\u0442\u0432\u0430 \u041f\u0412\u041e \u0420\u0424 \u043f\u0435\u0440\u0435\u0445\u0432\u0430\u0442\u0438\u043b\u0438 \u0434\u0432\u0430 \u0441\u043d\u0430\u0440\u044f\u0434\u0430 \u0420\u0421\u0417\u041e HIMARS \u0438 \u0441\u0431\u0438\u043b\u0438 42 \u0431\u0435\u0441\u043f\u0438\u043b\u043e\u0442\u043d\u0438\u043a\u0430 \u0412\u0421\u0423;\ud83d\udccc\u041f\u043e\u0442\u0435\u0440\u0438 \u0412\u0421\u0423 \u043d\u0430 \u044e\u0436\u043d\u043e\u0434\u043e\u043d\u0435\u0446\u043a\u043e\u043c \u043d\u0430\u043f\u0440\u0430\u0432\u043b\u0435\u043d\u0438\u0438 \u0437\u0430 \u0441\u0443\u0442\u043a\u0438 \u0441\u043e\u0441\u0442\u0430\u0432\u0438\u043b\u0438 \u0441\u0432\u044b\u0448\u0435 80 \u0432\u043e\u0435\u043d\u043d\u043e\u0441\u043b\u0443\u0436\u0430\u0449\u0438\u0445.", "6": "<b>Total Posts:</b> 33<br><b>Date:</b> 2023-11-12 14:05:10+00:00<br><b>Author:</b> tass_agency<br><b>Link:</b> https://t.me/s/tass_agency/218401<br><b>Subscribers:</b> 363503<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u0421\u043e\u0431\u0440\u0430\u043b\u0438 \u0433\u043b\u0430\u0432\u043d\u043e\u0435 \u0438\u0437 \u0437\u0430\u044f\u0432\u043b\u0435\u043d\u0438\u0439 \u0441\u043e\u0432\u0435\u0442\u043d\u0438\u043a\u0430 \u043f\u0440\u0435\u0437\u0438\u0434\u0435\u043d\u0442\u0430 \u0421\u0428\u0410 \u043f\u043e \u043d\u0430\u0446\u0438\u043e\u043d\u0430\u043b\u044c\u043d\u043e\u0439 \u0431\u0435\u0437\u043e\u043f\u0430\u0441\u043d\u043e\u0441\u0442\u0438 \u0414\u0436\u0435\u0439\u043a\u0430 \u0421\u0430\u043b\u043b\u0438\u0432\u0430\u043d\u0430 \u0442\u0435\u043b\u0435\u043a\u0430\u043d\u0430\u043b\u0443 CNN:\u25fe\ufe0f\u0421\u0428\u0410 \u0432\u044b\u0441\u0442\u0443\u043f\u0430\u044e\u0442 \u043f\u0440\u043e\u0442\u0438\u0432 \u0442\u043e\u0433\u043e, \u0447\u0442\u043e\u0431\u044b \u0431\u043e\u0435\u0432\u044b\u0435 \u0434\u0435\u0439\u0441\u0442\u0432\u0438\u044f \u0437\u0430\u0442\u0440\u0430\u0433\u0438\u0432\u0430\u043b\u0438 \u0431\u043e\u043b\u044c\u043d\u0438\u0446\u044b \u0413\u0430\u0437\u044b, \u0437\u0430\u044f\u0432\u0438\u043b\u0438 \u043e\u0431 \u044d\u0442\u043e\u043c \u0418\u0437\u0440\u0430\u0438\u043b\u044e;\u25fe\ufe0f\u0421\u0428\u0410 \u0443\u0447\u0430\u0441\u0442\u0432\u0443\u044e\u0442 \u0432 \u043f\u0435\u0440\u0435\u0433\u043e\u0432\u043e\u0440\u0430\u0445 \u043c\u0435\u0436\u0434\u0443 \u0418\u0437\u0440\u0430\u0438\u043b\u0435\u043c \u0438 \u041a\u0430\u0442\u0430\u0440\u043e\u043c \u043f\u043e \u0432\u043e\u043f\u0440\u043e\u0441\u0443 \u043e\u0431 \u043e\u0441\u0432\u043e\u0431\u043e\u0436\u0434\u0435\u043d\u0438\u0438 \u0443\u0434\u0435\u0440\u0436\u0438\u0432\u0430\u0435\u043c\u044b\u0445 \u0425\u0410\u041c\u0410\u0421 \u0437\u0430\u043b\u043e\u0436\u043d\u0438\u043a\u043e\u0432;\u25fe\ufe0f\u0411\u0435\u043b\u044b\u0439 \u0434\u043e\u043c \u043f\u043e\u0434\u0447\u0435\u0440\u043a\u043d\u0443\u043b, \u0447\u0442\u043e \u0418\u0437\u0440\u0430\u0438\u043b\u044c \u0434\u043e\u043b\u0436\u0435\u043d \u0441\u043e\u0431\u043b\u044e\u0434\u0430\u0442\u044c \u043f\u0440\u0430\u0432\u0438\u043b\u0430 \u0432\u0435\u0434\u0435\u043d\u0438\u044f \u0432\u043e\u0439\u043d\u044b \u0432\u043e \u0432\u0440\u0435\u043c\u044f \u043e\u043f\u0435\u0440\u0430\u0446\u0438\u0439 \u0432 \u0413\u0430\u0437\u0435;\u25fe\ufe0f\u0421\u0428\u0410 \u0441\u0447\u0438\u0442\u0430\u044e\u0442, \u0447\u0442\u043e \u043f\u0430\u043b\u0435\u0441\u0442\u0438\u043d\u0441\u043a\u0438\u0439 \u043d\u0430\u0440\u043e\u0434 \u0441\u0430\u043c \u0434\u043e\u043b\u0436\u0435\u043d \u0440\u0435\u0448\u0430\u0442\u044c, \u043a\u0442\u043e \u0438\u043c \u0431\u0443\u0434\u0435\u0442 \u0443\u043f\u0440\u0430\u0432\u043b\u044f\u0442\u044c, \u0432\u044b\u0441\u0442\u0443\u043f\u0430\u044e\u0442 \u043f\u0440\u043e\u0442\u0438\u0432 \u043f\u0440\u0438\u043d\u0443\u0434\u0438\u0442\u0435\u043b\u044c\u043d\u044b\u0445 \u043f\u0435\u0440\u0435\u043c\u0435\u0449\u0435\u043d\u0438\u0439 \u0436\u0438\u0442\u0435\u043b\u0435\u0439 \u0413\u0430\u0437\u044b;\u25fe\ufe0f\u0411\u0430\u0439\u0434\u0435\u043d \u0441\u0447\u0438\u0442\u0430\u0435\u0442 \u043e\u0434\u043d\u0438\u043c \u0438\u0437 \u0441\u0432\u043e\u0438\u0445 \u043f\u0440\u0438\u043e\u0440\u0438\u0442\u0435\u0442\u043e\u0432 \u0432\u043e\u0441\u0441\u0442\u0430\u043d\u043e\u0432\u043b\u0435\u043d\u0438\u0435 \u043a\u0430\u043d\u0430\u043b\u043e\u0432 \u0441\u0432\u044f\u0437\u0438 \u0432 \u0441\u0444\u0435\u0440\u0435 \u043e\u0431\u043e\u0440\u043e\u043d\u044b \u043c\u0435\u0436\u0434\u0443 \u0412\u0430\u0448\u0438\u043d\u0433\u0442\u043e\u043d\u043e\u043c \u0438 \u041f\u0435\u043a\u0438\u043d\u043e\u043c;\u25fe\ufe0f\u0411\u0430\u0439\u0434\u0435\u043d \u0438 \u0421\u0438 \u0426\u0437\u0438\u043d\u044c\u043f\u0438\u043d \u043e\u0431\u0441\u0443\u0434\u044f\u0442 \u044f\u0434\u0435\u0440\u043d\u0443\u044e \u043f\u0440\u043e\u0433\u0440\u0430\u043c\u043c\u0443 \u0418\u0440\u0430\u043d\u0430, \"\u0443\u0433\u0440\u043e\u0437\u044b\", \u043a\u043e\u0442\u043e\u0440\u044b\u0435 \u0422\u0435\u0433\u0435\u0440\u0430\u043d \u043f\u0440\u0435\u0434\u0441\u0442\u0430\u0432\u043b\u044f\u0435\u0442 \u0434\u043b\u044f \u0440\u0435\u0433\u0438\u043e\u043d\u0430 \u0438 \u0412\u0421 \u0421\u0428\u0410;\u25fe\ufe0f\u0414\u0436\u0435\u0439\u043a \u0421\u0430\u043b\u043b\u0438\u0432\u0430\u043d \u043e\u0442\u043a\u0430\u0437\u0430\u043b\u0441\u044f \u043e\u0442\u0432\u0435\u0447\u0430\u0442\u044c \u043d\u0430 \u0432\u043e\u043f\u0440\u043e\u0441 \u043e \u0442\u043e\u043c, \u0441\u043e\u0431\u043b\u044e\u0434\u0430\u0435\u0442 \u043b\u0438 \u0418\u0437\u0440\u0430\u0438\u043b\u044c, \u043f\u043e \u043c\u043d\u0435\u043d\u0438\u044e \u0412\u0430\u0448\u0438\u043d\u0433\u0442\u043e\u043d\u0430, \u043f\u0440\u0430\u0432\u0438\u043b\u0430 \u0432\u0435\u0434\u0435\u043d\u0438\u044f \u0432\u043e\u0439\u043d\u044b.", "7": "<b>Total Posts:</b> 16<br><b>Date:</b> 2023-11-12 13:20:29+00:00<br><b>Author:</b> itsdonetsk<br><b>Link:</b> https://t.me/s/itsdonetsk/114020<br><b>Subscribers:</b> 576593<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u0421\u0438\u0442\u0443\u0430\u0446\u0438\u044f \u043d\u0430 \u0434\u043e\u0440\u043e\u0433\u0435 \u0432 \u0414\u043e\u043d\u0435\u0446\u043a\u0435\u041f\u043e\u0434\u043f\u0438\u0441\u0430\u0442\u044c\u0441\u044f  |  \u041f\u0440\u0435\u0434\u043b\u043e\u0436\u0438\u0442\u044c \u043d\u043e\u0432\u043e\u0441\u0442\u044c", "8": "<b>Total Posts:</b> 15<br><b>Date:</b> 2023-11-12 05:09:15+00:00<br><b>Author:</b> ostashkonews<br><b>Link:</b> https://t.me/s/OstashkoNews/105402<br><b>Subscribers:</b> 361741<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \ud83d\udd34 \u0421\u0440\u0435\u0434\u0441\u0442\u0432\u0430 \u041f\u0412\u041e \u0443\u043d\u0438\u0447\u0442\u043e\u0436\u0438\u043b\u0438 \u0443\u043a\u0440\u0430\u0438\u043d\u0441\u043a\u0438\u0439 \u0431\u0435\u0441\u043f\u0438\u043b\u043e\u0442\u043d\u0438\u043a \u0441\u0430\u043c\u043e\u043b\u0435\u0442\u043d\u043e\u0433\u043e \u0442\u0438\u043f\u0430 \u043d\u0430\u0434 \u0411\u0435\u043b\u0433\u043e\u0440\u043e\u0434\u0441\u043a\u043e\u0439 \u043e\u0431\u043b\u0430\u0441\u0442\u044c\u044e", "9": "<b>Total Posts:</b> 15<br><b>Date:</b> 2023-11-12 16:01:59+00:00<br><b>Author:</b> swodki<br><b>Link:</b> https://t.me/s/swodki/320794<br><b>Subscribers:</b> 257477<br><b>Text:</b> \u0422\u0435\u043a\u0441\u0442: \u26a1\ufe0f\u0414\u0432\u043e\u0440\u043d\u0438\u043a \u0438\u0437 \u041f\u0435\u0442\u0435\u0440\u0431\u0443\u0440\u0433\u0430 \u0441\u043c\u0435\u0442\u0430\u0435\u0442 \u0432\u0435\u0441\u044c \u043c\u0443\u0441\u043e\u0440 \u0432 \u041c\u043e\u0441\u043a\u0432\u0435 \u043a \u0433\u043e\u0441\u0442\u0438\u043d\u0438\u0446\u0435 \u00ab\u0423\u043a\u0440\u0430\u0438\u043d\u0430\u00bb\u041c\u0438\u043d\u0443\u0442\u043a\u0430 \u044e\u043c\u043e\u0440\u0430"};

    function displayClusterText() {
        var selectedLabel = document.getElementById("clusterSelector").value;
        var details = clusterDetails[selectedLabel];
        var textDiv = document.getElementById("clusterTextDisplay");
        textDiv.innerHTML = '<p>' + details + '</p>';
        textDiv.classList.remove('hidden');
    }
</script>
