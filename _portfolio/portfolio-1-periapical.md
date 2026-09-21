---
title: "PeriApicaI: AI-Assisted Dental Radiology Prototype"
excerpt: "Experimental web prototype using Gemini Vision models for AI-assisted review of periapical radiographs.<br/><img src='https://img.shields.io/badge/Prototype-periapical.ai.studio-blue'> <img src='https://img.shields.io/badge/Methodology-AI--assisted_development_%26_prompt_design-purple'>"
collection: portfolio
lang: en
translation_key: portfolio-1-periapical
date: 2026-08-01
---

**Live URL:** [https://periapical.ai.studio](https://periapical.ai.studio)  
**Tools:** Google Gemini API (multimodal LLMs); I designed the workflow, the prompts and the review logic; the code was written with AI assistance  

### Overview
Dental radiology requires careful image interpretation, yet learners may not always have access to immediate feedback. I designed **PeriApicaI** as an experimental web prototype to explore whether multimodal AI could support learning from periapical radiographs. Developed from a clinician's perspective with AI-assisted development and prompt design, it provides automated technical-quality feedback and candidate finding annotations for educational review. The output is advisory; the project has not been clinically validated and is not a medical device.

### Recognition

**Top 500, AI Riser Vietnam 2026** — [Certificate of Completion](/files/AI_Riser_Vietnam_2026_Top_500_Nguyen_Bao_Trung.pdf) issued to Nguyen Bao Trung for participation with PeriApicaI.

### Key Features & Technical Approach

* **Two assessment workflows:** *Film Technical Error Check* covers 11 technical error types (receptor placement, angulation and geometry, exposure and processing; for example cone-cut and vertical elongation), and *Abnormality Detection & Segmentation* provides candidate pathology annotation across the project's defined taxonomy.
* **Optional dual-model comparison:** Can run Gemini Flash and Gemini Pro in parallel, compare their findings and polygon coordinates, and label agreement or review-required cases.
* **Validation and provenance:** Backend schemas normalize model output against dental dictionaries, while inference lineage and append-only human-review states keep model output separate from later review decisions.
* **Reliability controls:** Includes model fallback handling, execution limits, request cancellation with `AbortController`, and bounded recovery logic for transient failures.

### Learnings & Future Work
Developing PeriApicaI gave me hands-on experience with multimodal prompt design, model comparison, schema validation, and human-review workflows. **Future Work:** Evaluate the prototype with an appropriately governed, annotated dataset and independent clinical review before making any claims about performance or clinical use.
