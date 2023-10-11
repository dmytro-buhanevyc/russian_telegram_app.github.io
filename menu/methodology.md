---
layout: page
title: Methodology
permalink: /methodology
---

Our Telegram data analysis begins with the systematic scraping of designated Telegram channels to gather relevant data. Once this raw data is procured, it undergoes preprocessing to ensure its relevance and integrity.


<div class="wide-iframe-container">
    <iframe src="{{ site.baseurl }}/visualizations/2023-10-11/fig_pie_subs.html" width="120%" height="600" frameborder="0"></iframe>
</div>


The next phase involves the application of clusterization algorithms to group similar data, ensuring that related information is categorized correctly. The central component of this process is the utilization of the spatial clustering algorithm to group similar texts. The method is chosen for its proficiency in identifying clusters of varying shapes and sizes in large datasets.

<div class="gif-container">
    <img src="{{ site.baseurl }}/assets/images/clustering.gif?{{site.time | date: '%s%N'}}" alt="Description of GIF" />
</div>

For topic modeling, we employ a combination of n-grams and more advanced Natural Language Processing techniques. This allows us to discern overarching themes and recurring topics within the vast volume of content generated in Telegram channels.

Additionally, sentiment analysis techniques are deployed to gauge the tone and sentiment of the content.

Ethical Considerations: We prioritize the ethical implications of our work. The data is sourced from public Telegram channels and is used strictly for research purposes. No personal data is exploited. Furthermore, all research endeavors align with the principles of responsible and ethical data use.
