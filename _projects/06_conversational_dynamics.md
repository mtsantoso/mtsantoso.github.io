---
layout: page
title: Conversational Dynamics in Social VR
description: A Large-Scale, Longitudinal Study of Speech Acts and Nonverbal Behavior
img: assets/img/project_6_image_3.jpg
importance: 6
category: design
---

## Conversational Dynamics in Social VR: A Large-Scale, Longitudinal Study of Speech Acts and Nonverbal Behavior

**Role:** Lead Researcher, Full-Stack Data Pipeline Owner  
**Goal:** Build the first behavioral taxonomy of spoken communication in social VR — grounding it in both verbal intent and nonverbal kinematics — to produce a sharable dataset and design framework for understanding how people communicate inside immersive AI and social platforms.

### Project Summary

Social VR platforms like Horizon Worlds and ENGAGE are growing rapidly, yet almost nothing was empirically known about how people speak to each other inside them. This study filled that gap by building VRIDS (Virtual Reality Interaction Dynamics Scheme), a 10-category behavioral coding framework developed from the ground up for immersive social environments. We analyzed 9,738 spoken discourse units from 109 participants across 4 weeks of weekly metaverse classroom discussions, linking each turn-level speech act to 6DOF head and hand movement data collected at 30 Hz. The result is both a theoretical contribution (a validated taxonomy of VR communication) and a practical one: an annotated dataset designed to train LLMs to automatically recognize speech acts in social VR.

### The Challenge

**Problem:** Existing speech act coding schemes were built for face-to-face or text-based contexts. None accounted for the defining features of social VR: shared virtual objects that can be manipulated mid-conversation, avatar-mediated embodiment, spatial audio, and the blended affordances of FTF and CMC communication. When applied to our VR corpus, all eight prior schemes failed to capture the full range of observed communicative behaviors.

Without a VR-native taxonomy, product teams building social and collaborative AI experiences have no validated behavioral vocabulary for understanding what users are doing conversationally, how their behavior changes over time, or how verbal intent maps to physical expression in the headset.

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_6_image_1.jpg" class="img-fluid rounded z-depth-1" %}
</div>

**Users:** 109 undergraduate students enrolled in a 10-week Stanford course on virtual reality, meeting weekly in small groups (2–5 members) on the ENGAGE social VR platform using Meta Quest 2 headsets.

### Research Questions

1. What speech acts do people use to communicate in social VR groups?
2. How do those speech acts relate to nonverbal body movement?
3. How do speech act patterns change longitudinally as users gain familiarity?
4. What are the attractor and repeller states — conversational patterns groups gravitate toward or exit quickly?

### Methods & Data Pipeline

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_6_image_2.jpg" class="img-fluid rounded z-depth-1" %}
</div>

- **Audio extraction and transcription:** 93 session recordings extracted and transcribed via Otter.ai (85–90% accuracy). Four coders manually reviewed all transcripts against session video — a process requiring 7 weeks.
- **Discourse unitization:** All transcripts unitized into turn-level discourse units. Total corpus: 9,738 turns across 42.3 hours of audio.
- **Codebook development:** Bottom-up taxonomy developed by reviewing all 93 session videos and comparing against 8 prior coding schemes. Final VRIDS codebook contains 10 speech act categories, including two novel constructs absent from all prior schemes.
- **Coding procedure:** Three independent coder pairs coded all turns; inter-rater reliability ranged from κ = 0.66 to κ = 1.00 (mean κ = 0.99). Total coding effort: 2,790 hours across 9 coders.
- **Nonverbal data:** Head translation, head rotation, and hand movement captured at 30 Hz per participant and linked to concurrent speech act turns.
- **Statistical analysis:** Linear growth models (R, lme4), linear mixed models, and first-order Markov chain transition matrices (Python).

### Key Insights

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_6_image_3.jpg" class="img-fluid rounded z-depth-1" %}
</div>

**1. Questions are the dominant early behavior and decline with familiarity.** Questions decreased significantly over time (−0.64 per week, p < .05), mirroring the "learning about VR before learning in VR" effect.

**2. Context-dependent commentary is VR-native and grows over time.** Commentary on shared virtual objects — absent from all prior coding schemes — increased significantly over 4 weeks (+0.69 per week, p < .01).

**3. Idea sharing increases as questions decrease.** Ideation increased significantly (+0.37 per week, p < .01), confirming that once clarifying questions are resolved, collaborative idea generation expands.

**4. Head and hand movements track communicative intent.** Head translation, head rotation, and hand movement all predicted questioning (all p < .01). During conflict, users physically stilled — demonstrating that 6DOF behavioral data is a meaningful real-time signal for inferring user communicative state.

**5. Conversations self-organize into attractor and repeller states.** Questions attracted more questions (45% probability), context commentary attracted more context commentary (43%), and opinions attracted more opinions (41%). Disagreements and advice were repellers — groups moved through them quickly, returning to opinion-sharing.

### Design Opportunities

**1. Speech-Act-Aware AI Facilitation in Social VR**  
The VRIDS taxonomy provides a behavioral grammar that AI facilitators or moderation systems could use in real time — distinguishing questioning from ideation from disagreement, and adaptively scaffolding the interaction accordingly.

**2. 6DOF Kinematics as a Real-Time Intent Signal**  
Head and hand movement patterns significantly predicted speech act category even before the turn was completed. For AI systems in social VR, nonverbal behavioral data could serve as a low-latency predictor of communicative intent, enabling proactive rather than reactive interface responses.

**3. Designing for the Question-to-Ideation Transition**  
The longitudinal trajectory suggests a predictable onboarding arc for new users. Interface designs could explicitly support this arc — orienting users in early sessions to accelerate the transition to productive, idea-generating discussion.

**4. LLM Training Data for Speech Act Classification**  
The annotated VRIDS dataset — 9,738 labeled discourse turns linked to speaker, group, week, and nonverbal kinematics — is explicitly designed to train LLMs to recognize speech acts in social VR. This is a rare ground-truth corpus where verbal intent is taxonomized, validated to near-perfect inter-rater agreement, and paired with behavioral data.

*Full paper available at [doi.org/10.1016/j.chb.2025.108691](https://doi.org/10.1016/j.chb.2025.108691).*