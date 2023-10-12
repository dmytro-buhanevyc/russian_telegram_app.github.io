---
layout: page
title: Methodology
permalink: /methodology
---

Our Telegram data analysis begins with the systematic scraping of designated Telegram channels to gather relevant data. Once this raw data is procured, it undergoes preprocessing to ensure its relevance and integrity.


<style>
.wide-iframe-container {
    width: calc(100% + 20vw);  /* Reduced extra width */
    margin-left: -10vw;  /* Adjusted margin-left to shift container to the left */
    overflow: hidden;  /* Hide overflow */
}

.wide-iframe-container iframe {
    display: block;  /* Block display */
    margin: 0 auto;  /* Center iframe within container */
}
</style>

<div class="wide-iframe-container">
    <iframe src="{{ site.baseurl }}/visualizations/2023-10-11/fig_pie_subs.html" width="100%" height="830" frameborder="0"></iframe>
</div>



The next phase involves the application of clusterization algorithms to group similar data, ensuring that related information is categorized correctly. The central component of this process is the utilization of the spatial clustering algorithm to group similar texts. The method is chosen for its proficiency in identifying clusters of varying shapes and sizes in large datasets.

<img src='https://i.pinimg.com/originals/bb/3d/5e/bb3d5e522cbcb2dd07a81f8118de2041.gif' alt='DBSCAN visualization' />


For topic modeling, we employ a combination of n-grams and more advanced Natural Language Processing techniques. This allows us to discern overarching themes and recurring topics within the vast volume of content generated in Telegram channels. As an example of each topic we provide the 'central' text, one that has the lowest Euclidean distance to all neighbours in its designated cluster.
<div style="text-align: center;">
<img src='https://miro.medium.com/v2/resize:fit:1274/1*Nx6IyGfRAV1ly6uDGnVCxQ.gif' width='50%' height='50%' alt='Euclidean distance' />
</div>


Additionally, sentiment analysis techniques are deployed to gauge the tone and sentiment of the content.

Ethical Considerations: We prioritize the ethical implications of our work. The data is sourced from public Telegram channels and is used strictly for research purposes. No personal data is exploited. Furthermore, all research endeavors align with the principles of responsible and ethical data use.
