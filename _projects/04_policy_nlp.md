---
layout: page
title: Scalable Global Policy Surveillance
description: Auditing Global Platform Safety using Vertex AI & Large-Scale NLP
img: assets/img/project_4_image_1.jpg
importance: 4
category: design
---

## Scalable Global Policy Surveillance: Auditing Global Platform Safety using Vertex AI & Large-Scale NLP

**Role:** NLP Data Lead (Model Training & Content Analysis), Research Assistant  
**Goal:** Leveraging Vertex AI to evaluate global enforcement of Google's Content Policy

### Project Summary

This study evaluated the real-world impact of Google's June 2022 Inappropriate Content Advertising Policy update, which targeted discriminatory skin-lightening ads. I coordinated the collection and analysis of over 5,000 ads across eight countries. By establishing a Gold Standard database and training five NLP models, we identified significant shifts in ad content and discovered that Vertex AI was the most effective tool for identifying policy-violating content in a global, multilingual context.

### The Challenge

**The Policy Gap:** Automated safety filters often struggle with the nuance of discriminatory versus cosmetic language. Companies frequently evade policies by shifting terminology (e.g., moving from "whitening" to "brightening").

**User Needs:** Vulnerable populations — specifically global youth — need protection from harmful products that promote colorism and carry health risks such as mercury exposure.

**Business Requirements:** Google required an audit to assess whether their policy update changed the types of ads appearing in search results across diverse global markets.

**Technical Constraints:** Analyzing thousands of ads from eight countries (Bahamas, Germany, India, Malaysia, Mexico, South Africa, UAE, USA) required a model that understood cross-cultural linguistic nuances.

### Solution

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_4_image_1.jpg" class="img-fluid rounded z-depth-1" %}
</div>

We employed a rigorous mixed-methods and NLP pipeline to audit the policy's effectiveness:

- **Establishing the Gold Standard:** Worked with a team of coders to manually label 707 ads, categorizing them by product type and target demographics.
- **Model Benchmarking:** Trained and compared five NLP models. Vertex AI emerged as the top performer with the highest F1 score.
- **Global Comparative Analysis:** Applied the trained model to the full dataset (1,974 pre-policy and 3,262 post-policy ads) to measure changes in ad frequency and content strategies globally.
- **Multivariable Logistic Modeling:** Used statistical modeling to determine if specific keywords (e.g., "fairness," "superiority") significantly decreased after policy enforcement.

### Key Insights

Vertex AI successfully identified policy-violating content with high precision, providing a scalable way to monitor global ad ecosystems with a precision and recall score of 0.87.

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_4_image_2.jpg" class="img-fluid rounded z-depth-1" %}
</div>

While the policy achieved an overall reduction in specific harmful ad labels — including a 47% decrease in "Racial or Ethnic Identification" and a 66% decrease in "Natural Ingredients" claims — significant regional disparities emerged:

**Germany:** More straightforward impacts, including a decrease in labels related to specific formulation ingredients.

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_4_image_3.jpg" class="img-fluid rounded z-depth-1" %}
</div>

**India:** Despite the policy, ads remained prevalent by shifting focus. While labels for "Claimed Dermatological Benefits" declined, there was a simultaneous increase in ads targeting specific dermatological regions such as the face.

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_4_image_4.jpg" class="img-fluid rounded z-depth-1" %}
</div>

### Design Recommendations

Using these insights to refine the zero-shot classification capabilities of newer LLMs like Gemini to detect harmful content without requiring massive labeled datasets for every new region.

*Full results available at [doi.org/10.1016/j.amepre.2024.08.006](https://doi.org/10.1016/j.amepre.2024.08.006).*