---
title: "Medical VLM Exploration: Vision-Language Models for Healthcare"
date: 2025-06-01
summary: "Personal exploration of vision-language models applied to medical imaging. Reproduced CT-CLIP (chest CT contrastive VLM) and studied self-supervised learning, inference constraints, and deployment implications for clinical AI."
tags:
  - Research
  - Exploration
tech_stack:
  - PyTorch
  - Vision-Language Models
  - Self-supervised Learning
featured: false
status: "Personal Exploration"
role: "Independent"
duration: "2025"
highlights:
  - "Reproduction of CT-CLIP: contrastive vision-language model for chest CT images"
  - "Study of contrastive and self-supervised learning for volumetric medical data"
  - "Analysis of inference constraints and deployment implications in clinical AI"
  - "Exploration of interpretability and bias considerations in medical VLMs"
---

## Overview

A personal exploration investigating how vision-language models (VLMs) can be applied to medical imaging — specifically chest CT. Motivated by growing interest in foundation models for scientific and clinical data, and by the desire to understand the gap between research results and real-world clinical deployment.

## Approach

1. **Literature review** — surveyed recent VLMs adapted for medical imaging (BioViL, MedCLIP, CT-CLIP, and related work)
2. **CT-CLIP reproduction** — implemented and ran the CT-CLIP contrastive learning framework on chest CT data to understand architecture decisions and training dynamics
3. **Constraints analysis** — explored the practical gap between research performance and clinical deployment: data privacy, interpretability, regulatory considerations, and inference cost

## What I learned

- Contrastive and self-supervised learning methods and their adaptation to volumetric (3D) medical data
- Practical constraints of deploying VLMs in healthcare contexts (interpretability, regulatory, bias)
- How domain-specific evaluation differs from standard vision benchmarks

> Personal learning project — no production deployment or public repository.
