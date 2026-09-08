---
title: "Exploratory 3D Craniofacial Analysis"
excerpt: "Exploratory Python workflow using TotalSegmentator and NiBabel with 3D NIfTI data.<br/><img src='https://img.shields.io/badge/Tech-TotalSegmentator_%7C_NiBabel_%7C_Python-purple'>"
collection: portfolio
date: 2026-07-17
---

**Project Repository (Google Drive):** [View Notebooks & Data](https://drive.google.com/drive/folders/1M2Ebwdb7axTtll17ci1lYitd3eLlkHBu?usp=sharing)  
**Tech Stack:** Python, TotalSegmentator, NiBabel, Pandas, Matplotlib  

### Overview
Anatomical studies can involve slow manual segmentation. To learn about medical image processing, I experimented with TotalSegmentator on 3D NIfTI data and inspected the resulting structures and measurements. This was an early hands-on exercise in applying an existing deep-learning tool to craniofacial data.

### Motivation
While collecting data for research, I realized that manually masking CBCT slices is incredibly inefficient. I wanted to step out of my clinical routine and explore open-source deep learning tools that could automate this tedious process.

### Technical Approach
* Configured a Python environment to run TotalSegmentator on NIfTI volumes.
* Explored extraction of structures such as the skull, mandible, teeth, and airway-related regions.
* Calculated example volumes and generated 2D projections from segmented 3D arrays.

### Key Learnings & Future Work
Gained practical exposure to running an existing segmentation tool and handling 3D medical arrays with NiBabel. **Future Work:** Assess segmentation quality and, if appropriate, connect the workflow to statistical shape analysis for orthodontic research.
