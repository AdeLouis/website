---
title: Classification of Level of Consciousness in a Neurological ICU Using Physiological Data
summary: In this work, I ask the question, "can the level of consciousness in a population with brain hemorrhage be classified using physiological signals?"
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
url_code: "https://github.com/health-ai-lab/consciousness-classification"
url_pdf: "https://link.springer.com/article/10.1007/s12028-022-01586-0"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

**Background** Impaired consciousness is common in intensive care unit (ICU) patients, and an individual’s degree of consciousness is crucial to determining their care and prognosis. However, there are no methods that continuously monitor consciousness and alert clinicians to changes. We investigated the use of physiological signals collected in the ICU to classify levels of consciousness in critically ill patients.

**Methods** We studied 61 patients with subarachnoid hemorrhage (SAH) and 178 patients with intracerebral hemor- rhage (ICH) from the neurological ICU at Columbia University Medical Center in a retrospective observational study
of prospectively collected data. The level of consciousness was determined on the basis of neurological examination and mapped to comatose, vegetative state or unresponsive wakefulness syndrome (VS/UWS), minimally conscious minus state (MCS−), and command following. For each physiological signal, we extracted time-series features and performed classification using extreme gradient boosting on multiple clinically relevant tasks across subsets of physiological signals. We applied this approach independently on both SAH and ICH patient groups for three sets of variables: (1) a minimal set common to most hospital patients (e.g., heart rate), (2) variables available in most ICUs (e.g., body temperature), and (3) an extended set recorded mainly in neurological ICUs (absent for the ICH patient group; e.g., brain temperature).

**Results** On the commonly performed classification task of VS/UWS versus MCS−, we achieved an area under the receiver operating characteristic curve (AUROC) in the SAH patient group of 0.72 (sensitivity 82%, specificity 57%; 95% confidence interval [CI] 0.63–0.81) using the extended set, 0.69 (sensitivity 83%, specificity 51%; 95% CI 0.59–0.78) on the variable set available in most ICUs, and 0.69 (sensitivity 56%, specificity 78%; 95% CI 0.60–0.78) on the minimal set. In the ICH patient group, AUROC was 0.64 (sensitivity 56%, specificity 65%; 95% CI 0.55–0.74) using the minimal set and 0.61 (sensitivity 50%, specificity 80%; 95% CI 0.51–0.71) using the variables available in most ICUs.

**Conclusions** We find that physiological signals can be used to classify states of consciousness for patients in the ICU. Building on this with intraday assessments and increasing sensitivity and specificity may enable alarm systems that alert physicians to changes in consciousness and frequent monitoring of consciousness throughout the day, both of which may improve patient care and outcomes.
