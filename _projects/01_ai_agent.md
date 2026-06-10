---
layout: page
title: Personalizing AI Interactions
description: LLM Agent Conversations in Immersive Spaces
img: assets/img/project_1_image_1.jpg
importance: 1
category: design
---

## Personalizing AI Interactions: LLM Agent Conversations in Immersive Spaces

**Role:** Lead Researcher, Model Developer, Data Scientist, Immersive Environment UX Designer  
**Goal:** Evaluate how AI agent language and behavior influence environmental behavior



### Project Summary

This study investigates how psychological distance influences the way we feel about a politicized issue through AI agent interactions. By fine-tuning an AI agent to deliver ingroup vs. outgroup social statements and tailoring the virtual environment to be local vs. global, we investigate how users change their beliefs and actions about climate change. This work is the first to understand how AI can be implemented in immersive environments as a persuasive tool for global challenges.

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_1_image_1.jpg" class="img-fluid rounded z-depth-1" %}
</div>



### The Challenge

**Problem:** Climate change is often perceived as a distant threat — happening elsewhere, in the future, or to distant others — leading to inaction.

**User Needs:** Through user interviews, we identified that users need AI interactions that make the issue more relevant and urgent.

**KPIs:** Letter-writing to representatives and sharing news to those they know — both key to protective risk action and climate mitigation.

**Users:** 240 participants ranging from youth (13+) to adults (up to 80 years of age) of varying demographic and technological experience levels.


### The Agent and Immersive World

Using Unity, we developed an experimental virtual environment where users interact with an animal AI agent powered by Conv.ai and Microsoft Azure.

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_1_image_2.jpg" class="img-fluid rounded z-depth-1" %}
</div>

- **Model Behavior Fine-Tuning:** Using Conv.ai, I led development of the agent's communication model to deliver distinct social statement conditions — community-inclusive language for ingroup situations vs. outsider language for outgroup situations. The setup maintains a consistent persona while systematically shifting the distance of climate-related information to test behavioral nudges.

- **Multimodal Interaction Measurement:** Integrated 6DOF tracking of head and hand movements and speech data to capture real-time user reactions to agent prompts in Unity. Recorded and analyzed 9,000+ discourse units and audio data to identify real-time linguistic shifts in user responses.

- **Immersive Environment Design:** Curated immersive experience scenes through skyboxes to illustrate location changes, distal and proximal impacts of climate change, and facilitated time-travel in VR through scene changes.


### Key Insights

*All data analysis conducted in Python and R. All graphs generated using ggplot2 in R.*

**1.** Participants in the spatially distant condition were more likely to share a news article with someone they knew compared to those in a spatially close condition.

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_1_image_3.jpg" class="img-fluid rounded z-depth-1" %}
</div>

**2.** Participants talking to an AI agent using community-inclusive language had higher positive emotions in their letter compared to those talking to an agent with outsider language.

**3.** Participants talking to an AI agent using outsider language had higher head rotations compared to those talking to an agent using community-inclusive language.

---

*This work is currently under review at the Journal of Communication. Due to ethical reasons, we are unable to show the complete manuscript until peer review is completed. For questions, reach out to [Monique Santoso](mailto:mtsantoso@stanford.edu).*