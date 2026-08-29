---
title: "Medical Tabular Data Synthesis (CTGAN & ctdGAN)"
excerpt: "Conditional Tabular GANs for generating privacy-preserving synthetic demographic medical data.<br/><img src='https://img.shields.io/badge/Tech-Generative_AI_%7C_CTGAN-green'>"
collection: portfolio
date: 2026-06-15
---

**Project Repository (Google Drive):** [View Notebooks & Data](https://drive.google.com/drive/folders/1qInNhtiGobzpOIexIhhCxGZT5zZTeWID?usp=sharing)  
**Tech Stack:** Python, CTGAN, ctdGAN, Scikit-Learn, Differential Privacy  

### Overview
A major challenge in medical AI is the severe scarcity of open-source clinical datasets due to strict privacy laws. To learn about data privacy, I took my first steps in experimenting with CTGAN and ctdGAN to synthesize artificial demographic data (Age, Race, Sex). This exploratory project was a fascinating introduction to how researchers might eventually share data safely.

### Motivation
Reading AI research, I noticed how hard it is to access clinical datasets due to HIPAA and patient confidentiality. I became curious about how Synthetic Data Generation could solve this bottleneck without compromising patient privacy.

### Technical Approach
* Utilized the Synthetic Data Vault (SDV) ecosystem to train CTGAN and ctdGAN models.
* Fed a small sample of mock clinical demographic data to learn statistical distributions.
* Evaluated the synthesized data's fidelity and privacy metrics against the original dataset.

### Key Learnings & Future Work
Learned the fundamental concepts of Generative Adversarial Networks (GANs) and modern data anonymization strategies. **Future Work:** Explore synthesizing more complex clinical features (like diagnoses and treatment outcomes) while preserving underlying statistical relationships.
