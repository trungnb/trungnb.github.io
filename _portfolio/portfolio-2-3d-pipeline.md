---
title: "Prototype 3D-to-2D Craniofacial Shape Analysis"
excerpt: "Two-CBCT proof-of-concept testing compact multi-view craniofacial projections for potential forensic identification workflows.<br/><img src='https://img.shields.io/badge/Tech-TotalSegmentator_%7C_NiBabel_%7C_Python-purple'>"
collection: portfolio
lang: en
translation_key: portfolio-2-3d-pipeline
date: 2026-07-17
---

**Project Repository (GitHub):** [3D-Craniofacial-Pipeline](https://github.com/trungnb/3D-Craniofacial-Pipeline)  
**Tech Stack:** Python, TotalSegmentator, NiBabel, NumPy, Pandas  

### Overview
Two-CBCT proof-of-concept comparing compact 2D projections of segmented craniofacial anatomy with the corresponding 3D masks. The saved prototype runs test computational repeatability, comparison time, storage, and exploratory between-case overlap.

### Approach
* Segmented craniofacial structures, projected each mask into axial, coronal, and sagittal views, and compared 2D versus 3D outputs using timing, storage, Dice, and IoU.
* Found highly consistent repeated projections from the same scan and lower saved comparison cost for 2D outputs; with only two cases, this does not establish identification accuracy or clinical validity.
