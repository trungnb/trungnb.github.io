---
title: "PeriApicaI: AI Dental Radiography Platform"
excerpt: "Interactive clinical platform utilizing dual-mode Gemini Vision LLMs to diagnose periapical X-ray errors and segment pathologies.<br/><img src='https://img.shields.io/badge/Live_App-periapical.ai.studio-blue'> <img src='https://img.shields.io/badge/Methodology-Vibe_Coding_%26_Prompt_Eng-purple'>"
collection: portfolio
date: 2026-08-01
---

**Live URL:** [https://periapical.ai.studio](https://periapical.ai.studio)  
**Tech Stack:** Multimodal LLMs (Gemini Vision), Prompt Engineering, AI-Assisted Development (Vibe Coding)  

### Overview
Dental radiology requires intense pattern recognition, yet students often lack immediate feedback on X-ray errors due to scarce instructor time. To bridge this educational gap, I built **PeriApicaI**—an AI-powered web application serving as a virtual clinical tutor. Developed from a clinician's perspective using **AI-assisted development (vibe coding)** and rigorous **prompt engineering**, the platform rapidly evolved from an experimental prototype into a production-ready application. It evaluates uploaded periapical radiographs in real-time, providing instant technical feedback and pathology segmentation to help students and practitioners refine their diagnostic skills under strict clinical guardrails.

### Key Features & Technical Approach

* **Comprehensive Diagnostic Pipelines:** Supports both Technical Error Detection (e.g., cone-cutting, elongation) and Pathology Segmentation (identifying and mapping 8 distinct classes of dental lesions).
* **Dual-Model Consensus Architecture:** To ensure clinical reliability, the app runs parallel AI vision inferences (e.g., Gemini Pro & Flash). It cross-validates bounding polygons to filter out single-model hallucinations and tags findings with precise provenance ("Consensus" vs. "Review Required").
* **Semantic Validation & Provenance Tracking:** Robust backend schema validators intercept AI responses and enforce strict taxonomy mappings against established dental dictionaries. The system records immutable inference lineage, preserving exact AI model IDs, credentials, and original prediction confidence prior to human adjudication.
* **Production-Grade Infrastructure:** Engineered for stability and cost-efficiency with deterministic model fallback ladders, global execution budgets, asynchronous AbortControllers to prevent ghost requests, and a bounded offline-recovery queue for robust data syncing even under poor network conditions.

### Learnings & Future Work
Developing PeriApicaI provided deep experience in multimodal prompt engineering, deterministic AI orchestration, and mitigating LLM hallucination through strict bounding box intersection algorithms. **Future Work:** Establish a large-scale clinical pilot leveraging the platform's new human-review adjudication tools to fine-tune spatial accuracy with a dedicated, annotated dataset.
