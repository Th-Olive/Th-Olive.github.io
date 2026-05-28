---
title: "Thermal Satellite Super-Resolution GAN"
date: 2024-09-01
summary: "Conditional GAN fusing Sentinel-3 and Landsat thermal imagery to achieve ×33 resolution enhancement (1000 m → 30 m), reaching SSIM ≈ 98.8%. Part of the ESA-funded SENWISE project at Diginove."
tags:
  - Research
  - Geospatial
  - Deep Learning
tech_stack:
  - PyTorch
  - GANs
  - GDAL
  - Rasterio
  - Python
  - Docker
featured: true
status: "In Production / Research"
role: "R&D AI Engineer"
duration: "Sept 2024 – present"
highlights:
  - "×33 spatial resolution enhancement: 1000 m → 30 m thermal imagery"
  - "SSIM ≈ 98.8% on held-out test scenes"
  - "Conditional GAN architecture fusing Sentinel-3 SLSTR and Landsat-8/9 OLI-TIRS"
  - "End-to-end pipeline: data ingestion (GDAL/Rasterio) → training → production inference"
  - "ESA-funded research within the SENWISE programme"
  - "Sole contributor / project lead on Diginove's side"
  - "End-users: firefighters using thermal maps for fire monitoring"
  - "Poster presented at AI4EO 2025; paper in progress"
---

## Overview

**SENWISE** is an ESA-funded collaborative research project delivered through a consortium of partners. At Diginove, the work focused on the preparation of methods and use cases **ahead of the upcoming LSTM mission**, and the exploration of the future operational value of thermal Earth Observation for wildfire resilience.

## Challenges

A key challenge is that **current thermal satellite missions do not yet provide** the combination of high spatial and high temporal **resolution** expected from LSTM. Existing systems only cover part of that need: some observe the same area frequently but at coarse resolution, while others provide finer detail with much lower revisit frequency.

The project therefore had to create a **realistic proxy** for those future capabilities in order to study their potential usefulness in operational contexts such as fire-related monitoring.

## Approach

To address this limitation, the project relied on the **combination of complementary satellite missions**: Sentinel-3 for its high revisit frequency and Landsat 8/9 for its higher spatial resolution.

The core method relied on a **GAN-based spatio-temporal fusion** to reconstruct finer-resolution thermal imagery while preserving temporal relevance.

My contribution covered the full workflow:

- building and curating **large multisensor datasets**,
- designing preprocessing and data pipelines,
- developing and evaluating fusion models,
- benchmarking against existing spatio-temporal fusion methods,
- and integrating the resulting model into internal tools for practical use.

## Results

| Metric | Value |
|--------|-------|
| SSIM   | ≈ 98.8% |
| Resolution gain | ×33 (1000 m → 30 m) |

## Deployment

The inference pipeline runs on internal infrastructure. Data ingestion and pre-processing leverage GDAL and Rasterio for geospatial raster handling. The model is containerised with Docker for reproducible production deployment.

## Dissemination & Role

- Poster presented at **AI4EO 2025** (International Workshop on AI for Earth Observation)
- Paper currently in progress
- Led the project independently — sole contributor and internal point of contact on Diginove's side
- End-users include operational **firefighters** applying thermal maps for environmental fire monitoring

> This is a proprietary project — no public repository or live demo available.
