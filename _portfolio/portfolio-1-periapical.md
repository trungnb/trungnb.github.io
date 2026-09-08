---
title: "PeriApicaI: AI Dental Radiography Platform"
excerpt: "Experimental web prototype using Gemini Vision models for AI-assisted review of periapical radiographs.<br/><img src='https://img.shields.io/badge/Prototype-periapical.ai.studio-blue'> <img src='https://img.shields.io/badge/Methodology-AI--assisted_development_%26_prompt_design-purple'>"
collection: portfolio
lang: en
translation_key: portfolio-1-periapical
date: 2026-08-01
---

**Live URL:** [https://periapical.ai.studio](https://periapical.ai.studio)  
**Tech Stack:** Multimodal LLMs (Gemini Vision), Prompt Design, AI-Assisted Development  

### Overview
Dental radiology requires careful image interpretation, yet learners may not always have access to immediate feedback. I built **PeriApicaI** as an experimental web prototype to explore whether multimodal AI could support learning from periapical radiographs. Developed from a clinician's perspective with AI-assisted development and prompt design, it provides automated technical-quality feedback and candidate finding annotations for educational review. The output is advisory; the project has not been clinically validated and is not a medical device.

### Key Features & Technical Approach

* **Two assessment workflows:** Supports technical-quality review (for example, cone-cutting and elongation) and candidate pathology annotation across the project's defined taxonomy.
* **Optional dual-model comparison:** Can run Gemini Flash and Gemini Pro in parallel, compare their findings and polygon coordinates, and label agreement or review-required cases.
* **Validation and provenance:** Backend schemas normalize model output against dental dictionaries, while inference lineage and append-only human-review states keep model output separate from later review decisions.
* **Reliability controls:** Includes model fallback handling, execution limits, request cancellation with `AbortController`, and bounded recovery logic for transient failures.

### Learnings & Future Work
Developing PeriApicaI gave me hands-on experience with multimodal prompt design, model comparison, schema validation, and human-review workflows. **Future Work:** Evaluate the prototype with an appropriately governed, annotated dataset and independent clinical review before making any claims about performance or clinical use.
