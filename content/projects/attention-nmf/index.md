---
title: "Attention–NMF: Multispectral Document Analysis"
date: 2024-01-01
summary: "CNN attention encoder combined with an NMF decoder under a linear independence constraint for handwritten text extraction from ancient multispectral document images. Submitted to ICASSP 2025."
tags:
  - Research
  - Computer Vision
  - NLP
tech_stack:
  - PyTorch
  - CNNs
  - NumPy
  - Python
featured: true
status: "Published (ICASSP 2025)"
role: "Research Intern"
duration: "Jan 2024 – Aug 2024"
highlights:
  - "Novel Attention–NMF architecture combining learnable attention with non-negative matrix factorisation"
  - "Linear independence constraint on NMF basis vectors for improved source separation"
  - "Task: handwritten text extraction from ancient multispectral document images"
  - "Submitted and accepted to ICASSP 2025"
  - "Research conducted at Synchromedia Lab, ETS Montreal"
---

## Overview

Ancient multispectral document images present a challenging source separation problem: handwritten ink layers from different eras are visually entangled with paper texture, degradation artefacts, and background noise. Standard approaches fail because the spectral mixing is non-linear and the sources are highly correlated.

## Approach

I designed **Attention–NMF**, a hybrid architecture that combines:

1. **CNN attention encoder** — learns spatial and spectral attention maps to weight informative pixel-band combinations
2. **NMF decoder** — decomposes the attended representation into non-negative spectral components (interpretable basis vectors)
3. **Linear independence constraint** — a regularisation term that encourages NMF basis vectors to be linearly independent, reducing source confusion and improving separation quality

The model is trained end-to-end with a reconstruction objective plus the independence regulariser.

## Results

Attention–NMF outperforms standard NMF baselines and CNN-only approaches on handwritten text extraction benchmarks using multispectral document datasets from the Synchromedia Lab.

## Publication

Work submitted to and accepted at **ICASSP 2025** (IEEE International Conference on Acoustics, Speech and Signal Processing).

> Research paper in publication — no public repository available at this time.
