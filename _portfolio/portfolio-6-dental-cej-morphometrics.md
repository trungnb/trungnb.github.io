---
title: "Dental Morphometrics: CEJ & Crown-Root Ratio"
excerpt: "Quantitative Python analysis workflow for calculating Crown-Root ratios and identifying the Cementoenamel Junction (CEJ) from 3D dental models.<br/><img src='https://img.shields.io/badge/Tech-Python_%7C_Morphometrics-blue'>"
collection: portfolio
date: 2026-07-28
---

**Project Repository (Google Drive):** [View Notebooks & Data](https://drive.google.com/drive/folders/1IW2gQi0Azop_3Qrvm4e0FzrVchzdbBUQ?usp=sharing)  
**Tech Stack:** Python, Jupyter, Scikit-Image, Pandas, Data Visualization

### Overview
Manual 3D measurements in dentistry are highly tedious. Driven by a desire to learn basic computer vision, I wrote a proof-of-concept Python script to try and automate CEJ detection and crown-root ratio calculations from NIfTI files. While still in its early stages, this side project helped me grasp the fundamentals of algorithmic feature extraction.

### Motivation
Manually clicking through 3D dental models to find landmarks like the Cementoenamel Junction (CEJ) is incredibly time-consuming. I started this project to see if basic Python algorithms could do the heavy lifting and reduce human error.

### Technical Approach
* Loaded and manipulated 3D volumetric images (NIfTI format) using Python.
* Piloted basic edge detection and masking techniques to isolate tooth boundaries.
* Scripted experimental mathematical functions to calculate anatomical ratios (e.g., Crown-to-Root).

### Key Learnings & Future Work
Gained a foundational understanding of manipulating 3D arrays and voxel data in Python. **Future Work:** Aim to integrate these scripts with automated tooth segmentation models for a fully hands-off morphometric measurement pipeline.
