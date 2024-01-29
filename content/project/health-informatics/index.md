---
title: Predicting neurological outcome at ICU discharge
summary: In this work, I ask the question, "can patient data from the first two days in the ICU be used to predict neurological outcome at discharge?"
tags:
- ICU 
- classification
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
url_pdf: "https://github.com/AdeLouis/predicting-neurological-outcome/blob/main/Health-Informatics-Presentation.pdf"
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
To test whether vital signs and lab measurements from the first two days of admission in an intensive care unit (ICU) are predictive of the neurological outcome at discharge.

**Methods** I used data from patients in the MIMIC database with a diagnosis of traumatic brain injury and motor Glasgow Coma Scale (mGCS) recorded. Data included static, vital signs, and lab measurements from the first two days in the ICU. Motor GCS is used as a proxy to quantify neurological outcomes. This is mapped from a scale of 1 – 6: (i) 1, no response; (ii) 2, abnormal extension; (iii) 3, abnormal flexion; (iv) 4, flex to withdraw from pain; (v) 5, moves to localized pain; (vi) and 6, obeys command. We performed a binary classification task between the non-command following (1,2,3,4,5) vs command following (6) because this provides information about which patients could attain command following at discharge. We evaluate using recall, precision, and f1-score on three models: logistic regression, random forest, and XGBoost

**Results** The best f1 score of 0.66 was achieved on both logistic regression and XGBoost. The best average recall of 0.69 was attained using logistic regression, and the best average precision of 0.66 on XGBoost. Additionally, I found seven features that were deemed important across all models used.

**Conclusion** Results show that predicting the neurological outcome is a challenging task. This work has shown that using only static, vital signs, and lab measurements from the first two days in the ICU, we achieve an f1 score of 0.66. Future work could involve using more information such as drugs administered and exploring other ways to deal with missing values to retain more variables.
