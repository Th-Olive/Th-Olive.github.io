---
title: "Agent4EO: LLM-based Geospatial Agentic Workflow"
date: 2025-01-01
summary: "LLM routing agent (Ministral-3B via LangChain) that orchestrates geospatial EO tools to compute NDVI, LST, and dNBR metrics with OpenStreetMap context, then runs a second-pass LLM to generate operational narratives. Live demo on Hugging Face."
tags:
  - Research
  - Geospatial
  - NLP
tech_stack:
  - Python
  - Ministral-3B
  - LangChain
  - Rasterio
  - Gradio
featured: true
status: "Demo Available"
role: "Independent Exploration"
links:
  - icon: custom/huggingface
    name: "Hugging Face Demo"
    url: "https://huggingface.co/Th-Olive"
highlights:
  - "LLM routing agent powered by Ministral-3B via LangChain"
  - "Computes NDVI, LST, and dNBR geospatial metrics from satellite imagery"
  - "Integrates OpenStreetMap context for spatially-aware analysis"
  - "Second-pass LLM generates operational narratives for non-expert users"
  - "Agentic loop: natural-language query → tool selection → execution → interpretation"
  - "Live demo hosted on Hugging Face Spaces"
---

## Overview

Agent4EO is an independent exploration project investigating how large language models can act as orchestrators for geospatial and Earth Observation (EO) workflows. The agent receives a natural-language task (e.g. "detect vegetation change in this region between 2020 and 2023") and autonomously selects and sequences the appropriate tools to complete it.

## Approach

The agent is built around a **tool-use LLM** architecture powered by **Ministral-3B** via **LangChain**:

1. **Tool library** — Python functions computing key EO metrics: NDVI (vegetation health), LST (land surface temperature), dNBR (burn severity)
2. **OpenStreetMap integration** — enriches spatial context with road networks, land use, and administrative boundaries
3. **LLM routing orchestrator** — reasons over the task, selects and calls tools, interprets intermediate results
4. **Second-pass narrative LLM** — converts raw metrics and visualisations into human-readable operational summaries for non-expert end-users
5. **Gradio interface** — web UI for interactive querying and result display

## Motivation

Modern EO platforms provide powerful but fragmented APIs. An LLM agent acts as a unified interface — abstracting the complexity of individual tools and enabling domain experts (who may not be programmers) to run sophisticated geospatial analyses through natural language.

## Demo

A live demonstration is hosted on Hugging Face Spaces.
