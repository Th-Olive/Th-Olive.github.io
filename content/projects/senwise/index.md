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

SENWISE is an ESA-funded project at Diginove aimed at enhancing the spatial resolution of thermal satellite imagery for environmental monitoring applications. The core challenge: Sentinel-3 provides thermal data at 1000 m resolution while Landsat captures optical imagery at 30 m — a ×33 resolution gap that limits fine-grained land surface temperature analysis. The output is a **daily high-resolution thermal time series** — directly simulating future LSTM mission capabilities for operational land surface temperature (LST) monitoring.

## Challenges

The properties that make this problem technically non-trivial:
- **Spatial resolution mismatch (×33)**: the model must learn to generate fine spatial structure, not merely interpolate — requiring it to generalise across diverse land cover and seasonal conditions
- **Sensor heterogeneity**: Sentinel-3 SLSTR (thermal) and Landsat OLI-TIRS (optical) have different spectral responses, viewing geometries, and noise profiles, requiring cross-instrument alignment
- **Temporal misalignment**: acquisitions are not simultaneous; surface and atmospheric conditions change between passes, introducing domain shift the model must handle implicitly
- **Scale**: TB-scale EO archive processed via GDAL/Rasterio pipelines handling multi-resolution raster mosaicking, reprojection, and temporal compositing

## Approach

I designed and trained a **conditional GAN** that learns to generate high-resolution (30 m) thermal maps conditioned on:
- Low-resolution Sentinel-3 SLSTR thermal input
- High-resolution Landsat optical bands (as spatial guidance)

The generator uses a U-Net-style encoder-decoder with skip connections, while the discriminator enforces spectral and spatial consistency.

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
