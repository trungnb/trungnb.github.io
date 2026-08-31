---
title: "PeriApicaI: AI Dental Radiography Platform"
excerpt: "Interactive clinical platform utilizing dual-mode Gemini Vision LLMs to diagnose periapical X-ray errors and segment pathologies.<br/><img src='https://img.shields.io/badge/Live_App-periapical.ai.studio-blue'>"
collection: portfolio
date: 2026-08-01
---

**Live URL:** [https://periapical.ai.studio](https://periapical.ai.studio)  
**Tech Stack:** Multimodal LLMs (Gemini Vision), React/TypeScript, Prompt Engineering, Firebase  

### Overview
Dental radiology requires intense pattern recognition, yet students often lack immediate feedback on X-ray errors due to scarce instructor time. To bridge this educational gap, I built **PeriApicaI**—an AI-powered web application that serves as a virtual clinical tutor. The platform evaluates uploaded periapical radiographs in real-time, providing instant technical feedback and pathology segmentation to help students and practitioners refine their diagnostic skills.

### Key Features & Technical Approach

* **Comprehensive Diagnostic Pipelines:** The platform supports both Technical Error Detection (e.g., cone-cutting, elongation) and Pathology Segmentation (identifying and mapping 8 distinct classes of dental lesions).
* **Dual-Model Consensus Architecture:** To ensure clinical reliability, the app runs parallel AI vision inferences (e.g., Gemini Pro & Flash). It cross-validates bounding polygons to filter out single-model hallucinations and tags findings with precise provenance ("Consensus" vs. "Review Required").
* **Semantic Validation Engine:** Robust backend schema validators intercept AI responses, clamp confidence scores, and enforce strict taxonomy mappings against established dental dictionaries, preventing unformatted or hallucinatory outputs from reaching the user.
* **Resilient Infrastructure:** Engineered for stability and cost-efficiency with global execution budgets, asynchronous AbortControllers to prevent ghost requests, and a bounded offline-queue for robust data syncing even under poor network conditions.

### Learnings & Future Work
Developing PeriApicaI provided deep experience in multimodal prompt engineering and mitigating LLM hallucination through strict bounding box intersection algorithms and schema validation. **Future Work:** Aim to refine spatial accuracy via fine-tuning techniques using a dedicated, clinically-annotated dataset of dental radiographs.
