---
title: "PeriApicaI: AI Dental Radiography Platform"
excerpt: "Interactive clinical platform utilizing dual-mode Gemini Vision LLMs to diagnose periapical X-ray errors and segment pathologies.<br/><img src='https://img.shields.io/badge/Live_App-periapical.ai.studio-blue'>"
collection: portfolio
date: 2026-08-01
---

**Live URL:** [https://periapical.ai.studio](https://periapical.ai.studio)  
**Tech Stack:** Multimodal LLMs (Gemini Vision), React/TypeScript, Prompt Engineering, Firebase  

### Overview
Noticing that dental students often lack immediate feedback on X-ray errors due to scarce instructor time, I built PeriApicaI—a web application utilizing generative AI as a virtual tutor. Recently upgraded to v2.8.9, the platform now features a dual-model consensus pipeline and semantic guardrails for enhanced reliability in medical imaging contexts.

### Key Features & Technical Approach
* **Dual-Model Consensus Pipeline:** Runs parallel AI vision inferences (e.g., Gemini Pro & Flash) and cross-validates bounding polygons to filter out single-model hallucinations and tag findings with precise provenance ("Consensus" vs. "Review Required").
* **Semantic Validation Engine:** Implemented hard backend schema validators that intercept AI responses, clamp confidence scores, and enforce strict taxonomy mappings against established dental dictionaries.
* **Pathology Segmentation:** Extended the AI capabilities from basic technical errors (e.g., cone-cutting, elongation) to detecting 8-class dental pathologies with spatial polygon mapping.
* **Reliability Engineering:** Enforced global execution budgets with AbortControllers, preventing ghost requests and protecting API quotas while maintaining stable performance metrics.

### Learnings & Future Work
Developed deep experience in multimodal prompt engineering and mitigating LLM hallucination through strict bounding box mapping and schema validation. **Future Work:** Aim to refine spatial accuracy via fine-tuning techniques using a dedicated, clinically-annotated dataset.
