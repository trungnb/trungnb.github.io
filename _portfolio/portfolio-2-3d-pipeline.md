---
title: "3D Craniofacial Shape Analysis Pipeline"
excerpt: "Automated deep learning workflow using TotalSegmentator for processing 3D CBCT/CT scans.<br/><img src='https://img.shields.io/badge/Tech-TotalSegmentator_%7C_NiBabel_%7C_PyTorch-purple'>"
collection: portfolio
date: 2026-07-17
---

**Project Repository (Google Drive):** [View Notebooks & Data](https://drive.google.com/drive/folders/1M2Ebwdb7axTtll17ci1lYitd3eLlkHBu?usp=sharing)  
**Tech Stack:** Python, TotalSegmentator, NiBabel, PyTorch, Pandas  

### Overview
Anatomical studies are often bottlenecked by slow, manual CBCT segmentation. To learn about medical image processing, I experimented with TotalSegmentator to see if craniofacial extraction could be automated. These initial trials were my first hands-on lessons in applying deep learning to potentially speed up orthodontic data collection.

### Motivation
While collecting data for research, I realized that manually masking CBCT slices is incredibly inefficient. I wanted to step out of my clinical routine and explore open-source deep learning tools that could automate this tedious process.

### Technical Approach
* Configured a basic Python environment to run TotalSegmentator on dental CBCT scans (NIfTI format).
* Piloted the automated extraction of the skull, mandible, and individual teeth.
* Experimented with generating 2D orthogonal projections from the segmented 3D volumetric arrays.

### Key Learnings & Future Work
Gained practical exposure to terminal-based deep learning workflows and handling 3D medical arrays using NiBabel. **Future Work:** Aim to combine this automated segmentation step with statistical shape analysis pipelines for orthodontic research.
