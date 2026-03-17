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
  - "CPU-constrained deployment via ONNX and TensorRT runtime"
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

### Deployment constraints

- **CPU-only**: No GPU in production; models exported to ONNX and optimised via TensorRT for CPU inference
- **Legacy integration**: Inference called from C++ via the ONNX Runtime C++ API; Python training pipeline kept separate from the production runtime

## Results

- AI features deployed and actively used by end customers in production
- Primary use case: extraction of structured information from health record forms
- Reduced manual data entry for end users

> Proprietary project — no public repository available.
