---
title: Causal Effect of audio features on Chart Placement?
summary: Estimating the causal effects of audio features on higher chart placement on the billboard hot 100 charts
tags:
- Causal Inference
#date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

#image:
#  caption: Photo by rawpixel on Unsplash
#  focal_point: Smart

#links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_code: ""
url_pdf: "https://github.com/AdeLouis/causality-audio-chart-performance/blob/main/Causal-Inference-Presentation.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

**Objective** 
The way we consume music in recent years has changed from traditional mediums such as radio and physical sales to streaming via apps such as Spotify and Apple Music. This change is also reflected in the way the Billboard Hot 100 – the music chart that ranks the most popular songs in the country weekly – calculates its ranking by giving more weight to music streams. Performance on this chart is used as a proxy for artist success hence it is vital to understand what factors contribute to higher chart positions. In this work, we investigated whether audio features of tracks such as genre and tempo, have any causal effects on higher chart position (top 50) on debut.

**Methods and Materials**
We collected the past 5 years (2017-2021) of data (song title, artist name, and debut position) from Billboard charts for songs released in the summer and audio features of these songs from Spotify. To study the causal effects of the audio features on chart placement, we used a causal inference approach that computes the average causal significance for each of our features via pairwise testing while controlling for other potential audio features (causes). 

**Results**
 We found that features such as danceability, energy, r&b genre had positive causal effects while high-speechiness and duration had negative causal effects on higher chart placements. We further validated the relationships we found using a classification task where we trained a logistic regression model on data from 2017 to 2020 and tested on data from 2021. The model achieved an area under the receiver operating curve of 0.66.

**Conclusion**
 In this work, we investigated the causal effects of audio features on chart placement. In performing causal inference, we found features that had positively and negatively causal effects on our outcomes. Our results show that more work is needed to further understand the complex relationships associated with what makes songs chart higher.

