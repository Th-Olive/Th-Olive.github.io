---
title: "Document AI: Production AI for Document Management"
date: 2024-09-01
summary: "Integration of OCR, handwritten digit/character recognition, and BERT-based NER into a legacy document management system. C++/ONNX/TensorRT deployment on CPU-constrained hardware. Features in production for health records extraction."
tags:
  - Engineering
  - Research
tech_stack:
  - Python
  - C++
  - ONNX
  - TensorRT
  - BERT
  - OCR
featured: true
status: "In Production"
role: "R&D AI Engineer at Diginove"
duration: "Sept 2024 – present"
highlights:
  - "OCR integration for text extraction from scanned documents"
  - "Handwritten digit and character recognition models trained on target-domain data"
  - "Named Entity Recognition (BERT-based NER) for structured field extraction"
  - "CPU-only inference via ONNX and TensorRT — no GPU dependency in production"
  - "Integration into a legacy C++ document management system"
  - "Health records extraction feature deployed in production"
---

## Overview

An internal R&D workstream at Diginove focused on modernising a legacy document management system with AI-powered capabilities. The system serves customers who manage large volumes of structured and semi-structured documents, including health records and forms requiring structured information extraction.

## Problem

The existing system relied on deterministic, rule-based methods with limited flexibility. The goal was to integrate learned models capable of handling handwritten content, extracting structured entities, and operating reliably under production constraints — specifically: CPU-only inference and integration into an existing C++ codebase.

## Approach

I designed and integrated three AI components:

1. **OCR pipeline** — text recognition from scanned document images, integrated as a pre-processing stage
2. **Handwritten recognition** — models for digit and character recognition on form fields, trained on curated datasets representative of the target documents
3. **Named Entity Recognition** — BERT-based NER model fine-tuned to extract structured fields (names, dates, identifiers) from extracted text

### Production deployment

- **CPU-only inference**: all models exported to ONNX and optimised via TensorRT — no GPU dependency in production, a hard constraint met through careful model selection and export pipeline design
- **Legacy integration**: inference called from C++ via the ONNX Runtime C++ API; Python training pipeline kept fully decoupled from the production runtime

## Results

- Structured field extraction (names, dates, identifiers) from health record forms — previously manual, now automated end-to-end
- AI features deployed and actively used by end customers in production
- CPU-only deployment: no GPU dependency in the production environment, achieved via ONNX optimisation

> Proprietary project — no public repository available.
