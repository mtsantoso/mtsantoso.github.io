---
layout: page
title: The Relational Costs of Asymmetric MR
description: How Asymmetric Headset Use in Large Groups Shapes Social Perception and Collaboration
img: assets/img/project_7_image_1.jpg
importance: 7
category: design
---

## The Relational Costs of Asymmetric Mixed Reality Headset Use in Large Groups

**Role:** Lead Researcher, Study Designer, Quantitative Analyst  
**Goal:** Conduct the first large-group quantitative field study of how wearing a mixed reality headset in a co-present group shapes social perception, relational closeness, and collaborative behavior.

### Project Summary

As MR headsets enter classrooms, workplaces, and collaborative environments, real-world deployments are rarely symmetric — some people wear headsets while others in the same room do not. This study is, to our knowledge, the first large-group, quantitative experiment examining how asymmetric headset use shapes interpersonal perception. Using the Meta Quest 3 in passthrough-only mode, we assigned participants in groups of 9–10 to either wear a headset or not, then measured social presence, closeness, ostracism, and compromise behavior following a collaborative group decision-making task.

**Core finding:** Headset use creates a unidirectional perceptual burden — non-wearers feel less connected to and less present with headset-wearing group members, while headset wearers, retaining full visual access via passthrough, experience no parallel decline.

### The Challenge

**Problem:** MR headsets are optimized for the wearer's subjective experience. But in real-world deployments — hybrid classrooms, team meetings, design reviews — the same device that enhances the wearer's situational awareness silently degrades how their co-present partners perceive and relate to them.

The mechanism is structural and unidirectional: when a person puts on a headset, they lose very little. Their partners, however, lose access to the wearer's eye gaze, facial affect, upper-face expressiveness, and attentional focus — the primary nonverbal signals humans use to gauge whether someone is engaged, attending, and trustworthy. This cue asymmetry is not a mutual barrier; it is a tax paid exclusively by the people outside the device.

Prior work on this asymmetry was qualitative and limited to dyads. No large-group, controlled quantitative study existed. We addressed this directly.

### Study Design

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_7_image_1.jpg" class="img-fluid rounded z-depth-1" %}
</div>

101 university students, randomly assigned within groups of 9–10 to headset or no-headset conditions.

- **Task:** Groups completed the desert survival ranking task individually, then collaboratively to reach group consensus
- **Headset condition:** Meta Quest 3, passthrough-only mode (no virtual content; room visible through external cameras at 39ms latency, 120Hz)
- **Measures:** Social presence, ostracism, closeness (IOS scale), and behavioral measure of compromise
- **Pre-registered** hypotheses and analysis plan prior to data collection

### Key Findings

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_7_image_2.jpg" class="img-fluid rounded z-depth-1" %}
</div>

**1. Headset use reduces social presence — but only for people outside the headset.** Non-headset participants rated social presence toward headset-wearing group members significantly lower. Headset wearers showed no parallel decrease, confirming the unidirectional nature of the cue-restriction effect: the relational cost is paid by those outside the device, not by those inside it.

**2. Non-headset wearers felt significantly less close to headset-wearing partners.** Closeness was significantly lower toward headset-wearing group members for non-wearers, and familiarity robustly moderated this effect. For headset wearers, relational history substituted for real-time nonverbal access.

**3. A crossover pattern in group compromise behavior.** Among familiar participants, non-headset wearers compromised more. Among unfamiliar participants, headset wearers compromised more — likely a proactive signaling strategy to compensate for obscured nonverbal channels. This suggests participants actively adapt their collaborative behavior as a function of both hardware state and relational context.

### Design Implications for XR Products

**1. The headset-wearer's experience is not the whole experience.**  
Current XR product development centers the wearer. This study quantifies what the people around the wearer experience. For consumer and enterprise XR products deployed in co-present contexts, the social experience of non-wearers is a product metric that currently goes unmeasured — it should be a first-class design input.

**2. External social signaling is an underinvested feature surface.**  
The primary mechanism driving the social presence and closeness gaps is the loss of the wearer's eye gaze, facial expression, and attentional focus. External display surfaces — rendering gaze direction, emotional state, or a simplified presence indicator on the headset exterior — could restore the nonverbal signals that co-present partners currently lose.

**3. Familiarity should inform deployment sequencing.**  
The headset-induced relational gap is most acute when group members are unfamiliar. Organizations deploying MR for team collaboration should sequence device introduction after initial relationship formation. XR onboarding UX could explicitly scaffold this by recommending first-use scenarios that are lower-stakes for group cohesion before shared social activities.

*This paper is currently under review. For questions, reach out to [Monique Santoso](mailto:mtsantoso@stanford.edu).*