# The Generalization Crisis and the Forensic Triad

[![Paper](https://img.shields.io/badge/Paper-Springer%20LNNS-blue)](LINK_TO_PDF)
[![Venue](https://img.shields.io/badge/Venue-ICICT%202026-green)](https://icict.co.uk/)

This repository contains the taxonomy, literature mapping, and conceptual framework introduced in our survey: **"The Generalization Crisis and the Forensic Triad: A Comprehensive Survey of Deepfake Detection (2023-2025)."**

## 🛑 The Diagnosis: The Generalization Crisis
We document a catastrophic performance collapse in Phase I (Artifact-Centric) detectors. While these models achieve **99.2% AUC** on legacy benchmarks (FaceForensics++), they fail to **~50% (random)** when confronted with modern diffusion-based "in-the-wild" datasets.

## 🏗️ The Framework: The Forensic Triad
To move beyond binary classification, we propose the **Forensic Triad**:
1. **Attribution:** Identifying the generative source (GAN vs. Diffusion vs. Hybrid).
2. **Localization:** Spatial/Temporal mapping of forged regions.
3. **Explanation:** Providing physical or semantic evidence for the verdict.

## 📊 The 3-Phase Taxonomy
We categorized 40+ seminal papers (2023-2025) into three evolutionary tiers:
- **Phase I (Artifact-Centric):** Obsolete; focuses on GAN fingerprinting.
- **Phase II (Foundation-Adapted):** Current SOTA; leverages frozen weights (CLIP/Wav2Vec) for robustness.
- **Phase III (Semantic-Physical):** The Frontier; detecting reality violations (rPPG, shadows, physics).

## 📂 Repository Contents
- `/taxonomy`: Structured CSV/Markdown of all 40+ reviewed papers.
- `/taxonomy/surveyed_literature.bib`: BibTeX file for all surveyed literature.
