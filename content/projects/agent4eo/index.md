---
title: "Agent4EO: LLM-based Geospatial Agentic Workflow"
date: 2025-01-01
summary: "An LLM agent that integrates satellite image processing tools into an automated geospatial workflow. Enables natural-language-driven Earth Observation analysis via tool orchestration. Demo available on Hugging Face."
tags:
  - Research
  - Geospatial
  - NLP
tech_stack:
  - Python
  - LLMs
  - EO APIs
  - Tool Orchestration
featured: true
status: "Demo Available"
role: "Independent Exploration"
links:
  - icon: custom/huggingface
    name: "Hugging Face Demo"
    url: "https://huggingface.co/Th-Olive"
highlights:
  - "LLM agent with access to geospatial and EO processing tools"
  - "Natural-language interface for satellite image analysis tasks"
  - "Agentic tool orchestration: query → plan → execute → interpret"
  - "Exploration of LLM capabilities in Earth Observation workflows"
  - "Live demo hosted on Hugging Face Spaces"
---

## Overview

Agent4EO is an independent exploration project investigating how large language models can act as orchestrators for geospatial and Earth Observation (EO) workflows. The agent receives a natural-language task (e.g. "detect vegetation change in this region between 2020 and 2023") and autonomously selects and sequences the appropriate tools to complete it.

## Approach

The agent is built around a **tool-use LLM** architecture:

1. **Tool library** — a set of Python functions wrapping EO APIs (satellite data access, image processing, change detection, visualisation)
2. **LLM orchestrator** — reasons over the task, selects tools, interprets results, and decides next steps
3. **Agentic loop** — continues until the task is resolved or a stopping condition is met

This architecture mirrors patterns from the agent/function-calling literature applied to the domain of Earth Observation.

## Motivation

Modern EO platforms provide powerful but fragmented APIs. An LLM agent acts as a unified interface — abstracting the complexity of individual tools and enabling domain experts (who may not be programmers) to run sophisticated geospatial analyses through natural language.

## Demo

A live demonstration is hosted on Hugging Face Spaces.
