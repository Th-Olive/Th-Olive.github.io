---
title: "Medical VLM: Self-directed Study on Vision-Language Models for Healthcare"
date: 2025-06-01
summary: "Self-directed study of vision-language models for medical imaging. Reproduced CT-CLIP (contrastive VLM for chest CT), surveyed the field from BioViL to MedCLIP, and analysed the gap between research benchmarks and clinical deployment constraints."
tags:
  - Research
tech_stack:
  - PyTorch
  - Vision-Language Models
  - Self-supervised Learning
featured: true
external_link: "https://github.com/Th-Olive/CT-CLIP"
status: "Personal Study"
role: "Independent"
duration: "2025"
highlights:
  - "Surveyed medical imaging VLMs: BioViL, MedCLIP, CT-CLIP, and related contrastive learning approaches"
  - "Reproduced CT-CLIP: contrastive vision-language pre-training on chest CT — studied architecture, 3D data handling, and training dynamics"
  - "Analysed the gap between research benchmarks and clinical deployment: privacy, interpretability, regulatory constraints, inference cost"
  - "Active self-directed learning — motivated by interest in AI for healthcare and regulated environments"
---

## Context

A self-directed study investigating how vision-language models (VLMs) can be applied to medical imaging — specifically chest CT. Motivated by genuine interest in the intersection of AI and clinical practice, and by the question of what it actually takes to deploy a foundation model in a regulated, safety-critical environment.

This is not a production project and no clinical system was built. The goal was to build concrete understanding of the field: the architectures, the training approaches, the benchmarks, and the constraints that separate research results from clinical reality.

## Approach

1. **Literature review** — surveyed recent VLMs adapted for medical imaging: BioViL, MedCLIP, CT-CLIP, and related work on contrastive and self-supervised learning for clinical data
2. **CT-CLIP reproduction** — implemented and ran the CT-CLIP contrastive learning framework on chest CT data to understand architecture decisions, 3D volumetric data handling, and training dynamics at first hand
3. **Deployment analysis** — studied the practical gap between benchmark performance and clinical deployment: data privacy and de-identification, interpretability requirements, and inference cost under clinical infrastructure

## Takeaways

- How contrastive and self-supervised methods adapt to volumetric (3D) medical data — the data handling and augmentation challenges that don't appear in standard vision literature
- Why domain-specific evaluation in medical AI differs fundamentally from standard benchmarks — and why strong research metrics do not translate directly to clinical validity

> Self-directed learning project — no production deployment or public repository.
