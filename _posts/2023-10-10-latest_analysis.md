---
layout: post
title: "Russia Telegram Analysis"
author: "Dmytro Bukhanevych"
categories: your_category
tags: [your_tags]
image: cutting.jpg

---

<style>
    .iframe-container {
        width: 80%;       /* Setting width to 80% of parent's width */
        margin: 0 auto;  /* Centering the container */
        overflow: hidden; /* In case the iframe content spills over */
    }

    .iframe-container iframe {
        width: 100%;     /* Making the iframe take the full width of its container */
        border: none;    /* Removing any borders from the iframe */
    }
</style>

... Your content ...

<!-- Embedding Plotly Visualization -->
<!-- Embedding Plotly Visualization -->
<!-- Embedding Plotly Visualization -->
<!-- Using the iframe container -->
<div class="iframe-container">
    <iframe src="{{ site.baseurl }}/visualizations/fig_topics_time.html" height="800"></iframe>
</div>

<!-- Embedding the DataFrame table -->
<!-- Styles for the button -->
<style>
    .download-btn {
        display: inline-block;
        padding: 10px 20px;
        background-color: #f8f8f8;
        border-radius: 5px;
        box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
        text-decoration: none;
        color: #333;
        font-weight: bold;
        margin-bottom: 20px;
    }

    .download-btn img {
        vertical-align: middle;
        margin-right: 10px;
    }
</style>

<!-- Download button -->
<a href="{{ site.baseurl }}/visualizations/dataframe_table.html" download class="download-btn">
    <img src="{{ site.baseurl }}/path_to_your_mini_disk_image.png" alt="Download Icon"> Download the Table
</a>


... Rest of your content ...
