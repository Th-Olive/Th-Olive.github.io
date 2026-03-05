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
---

## Overview

SENWISE is an ESA-funded project at Diginove aimed at enhancing the spatial resolution of thermal satellite imagery for environmental monitoring applications. The core challenge: Sentinel-3 provides thermal data at 1000 m resolution while Landsat captures optical imagery at 30 m — a ×33 resolution gap that limits fine-grained land surface temperature analysis.

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

> This is a proprietary project — no public repository or live demo available.
