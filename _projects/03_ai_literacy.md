---
layout: page
title: AI Literacy & LLM Interaction
description: How AI Literacy Shapes Communication Trajectories in Human-LLM Interaction
img: assets/img/project_3_image_2.jpg
importance: 3
category: design
---

## AI Literacy Differentiates Longitudinal Style-Word Trajectories in Human-LLM Interaction

**Role:** Lead Researcher, Data Scientist  
**Goal:** Understand how sustained LLM interaction reshapes user communication behavior over time, and whether AI literacy moderates that change, to surface behavioral signals that can inform adaptive AI interface design.

### Project Summary

A 6-week longitudinal field study of 142 undergraduate students interacting weekly with a RAG-grounded LLM (VHIL-E) in a naturalistic educational setting. Using automated linguistic analysis (LIWC-22) and multilevel modeling, we tracked how pronoun use and language style evolved across 793 student–LLM exchanges, comparing high AI literacy users, low AI literacy users, and the LLM itself. This study produced the first empirical, field-based evidence that AI literacy produces divergent behavioral trajectories in human-LLM interaction.

### The Challenge

**Problem:** As LLMs become embedded in everyday workflows, a critical question emerges: does repeated AI interaction reshape how users communicate, and does it do so equitably? Prior work (Anthropic Economic Index, 2026) documented that experienced AI users collaborate more iteratively and achieve higher task success, but the psychological mechanisms underlying these differences remained unmeasured. If AI literacy systematically differentiates how users evolve their interaction style, interface designs built on a uniform user model may inadvertently widen the gap between power users and novices.

**Users:** 142 undergraduate students enrolled in a 10-week Stanford course on VR and AI.

### Research Design & Methods

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_3_image_1.jpg" class="img-fluid rounded z-depth-1" %}
</div>

- **Longitudinal within-subjects field study** embedded in a weekly course rhythm to maximize ecological validity
- Each week for 6 weeks, students submitted a structured query to VHIL-E and a paragraph-length written response, yielding 793 question-answer pairs
- **Text analysis:** All texts scored using LIWC-22, extracting six pronoun categories and a composite Linguistic Style Matching (LSM) score
- **Statistical modeling:** Linear mixed effects models per LIWC feature in R, including between-person baselines, within-person lagged parameters, group comparisons, and group × time interaction terms

### Key Findings

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_3_image_2.jpg" class="img-fluid rounded z-depth-1" %}
</div>

**1. High AI literacy users showed declining self-reference over time.** High-literacy students progressively reduced first-person singular pronoun use relative to the LLM. This divergence is consistent with cognitive offloading: as high-literacy users became more fluent in delegating tasks to the model, their outputs reflected a reduced personal stance.

**2. High AI literacy users shifted toward other-oriented language.** High-literacy students ended with significantly higher use of gendered third-person pronouns, suggesting a transition toward content- and author-focused engagement — mirroring findings on how experienced AI users shift toward professional rather than personal topics.

**3. Low AI literacy users showed a different trajectory.** Low-literacy students began with higher collective pronoun use but exhibited a negative trend over time, not developing the same cognitive offloading patterns as high-literacy users.

### Design Opportunities

**1. AI Literacy-Adaptive Onboarding and Scaffolding**  
LLM interfaces should detect early-stage interaction patterns and offer scaffolded prompting guidance, such as query reframing suggestions, complexity laddering, specifically calibrated for users not yet shifting toward task-focused engagement.

**2. Longitudinal User Behavioral Modeling**  
Pronoun use is a stable, within-person signal that predicts week-to-week behavior. Interfaces with ongoing interaction histories could use linguistic trajectory data and not just static profiles, to surface personalized recommendations or flag disengagement patterns early.

**3. Closing the Human-AI Style Gap**  
Neither student group matched the LLM's linguistic style even after 6 weeks. Prompting scaffolds, response formatting choices, or explicit translation of LLM output into registers closer to user style could reduce cognitive load, particularly for low-literacy users.

*This work is currently under review. For questions, reach out to [Monique Santoso](mailto:mtsantoso@stanford.edu).*