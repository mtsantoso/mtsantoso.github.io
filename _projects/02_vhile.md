---
layout: page
title: Algorithmic Trust & Reliability
description: Reducing LLM Hallucinations by 50% for High-Intent Power Users
img: assets/img/project_2_image_2.jpg
importance: 2
category: design
---

## Algorithmic Trust & Reliability: Reducing LLM Hallucinations by 50% for High-Intent Power Users

**Role:** Primary Researcher, Model Developer, Data Scientist  
**Goal:** Reducing LLM hallucinations through the "Seven Cs" RAG Framework and optimizing model outputs for high-frequency power users

### Project Summary

VHIL-E is a specialized Large Language Model designed to serve as an expert representative for Stanford's Virtual Human Interaction Lab. To combat AI hallucinations in scientific contexts, I led the development of a Retrieval-Augmented Generation (RAG) system and a 10-week longitudinal field study. By strictly constraining the model to a curated 2.3-million-word index, we matched student-level academic performance while reducing hallucinations by over 50%.

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_2_image_1.jpg" class="img-fluid rounded z-depth-1" %}
</div>

### The Challenge

**Problem:** General-purpose LLMs often produce hallucinations — confident but factually incorrect answers. In academic or scientific settings, these errors damage user trust and impede learning.

**User Needs:** Students and researchers required a tool that could accurately synthesize 20 years of lab research, lecture transcripts, and news articles without hallucinations.

**KPIs:** Accuracy rate exceeding 80% on expert benchmarks and a significant reduction in student-reported errors during live interactions.

**Users:** Students and researchers studying virtual reality.

### Solution: Retrieval-Augmented Generative Model Creation

<div class="row justify-content-center mt-3 mb-3">
  {% include figure.liquid path="assets/img/project_2_image_2.jpg" class="img-fluid rounded z-depth-1" %}
</div>

1. **Collecting & Cleaning:** Aggregated diverse data sources and manually cleaned transcripts to remove noise.
2. **Classifying & Chunking:** Categorized data by source type and broke the 2.3M words into ~10,000 manageable semantic chunks.
3. **Creating & Correlating:** Generated numerical embeddings for the chunks to build a searchable vector index.
4. **Connecting & Testing:** Connected the index to GPT-4o and GPT-5, testing two conditions — Base/RAG Hybrid (general training + index) and RAG Constrained (index only).

### Model Evaluation

The study used a longitudinal within-subjects design embedded into a weekly course rhythm to stress-test reliability. Both conditions were standardized on GPT-5, uniform chunk length, and top 5 most relevant chunks returned.

**Phase 1: User Testing (Weeks 2–9)**
Students queried the Base/RAG Hybrid model weekly until it produced a verifiably wrong answer.

**Phase 2: Comparative Product Evaluation (Week 10)**
Students selected their most egregious wrong answer from 8 weeks of logs, re-confirmed it as a hallucination, then tested the same question in the RAG-Constrained model.

### Key Insights

*All data analysis conducted in R.*

- **Base/RAG Hybrid Hallucination Rate:** 69.7% of responses flagged as egregious
- **RAG-Constrained Hallucination Rate:** Only 32.6% flagged
- **Impact:** Strictly limiting the model's search space to the verified index reduced egregious hallucinations by over 50%, demonstrating that grounding is a critical prerequisite for user trust in expert systems

### Design Opportunities

- **Groundedness Toggle:** Allow users to lock responses to a specific uploaded knowledge base for fact-critical tasks, with clear visual citations for every claim
- **Pre-Retrieval Cleaning Tools:** Provide an automated data health check that flags messy formatting before the model indexes it

*To read the published academic paper, visit [doi.org/10.1177/21522715261423752](https://doi.org/10.1177/21522715261423752).*