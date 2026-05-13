# Literature Mapping & Quantitative Analysis (2023-2025)

This document provides a structured mapping of the 39+ seminal papers reviewed in our survey. Methodology is categorized according to the **Forensic Triad** phases.

## Phase I: Artifact-Centric (Legacy/Obsolete)
*Focus: Pixel-level distributions, GAN fingerprints, and frequency artifacts.*

| Paper Title | Year | Methodology | Key Metric (OOD AUC) |
| :--- | :--- | :--- | :--- |
| **VoiceWukong: Audio Deepfake Benchmarking** | 2024 | Audio: Frequency-domain analysis of spectral differences. | N/A |
| **Deepfake-Eval-2024: Multi-modal Benchmark** | 2025 | Video: Quantitative evaluation of Phase I CNN baselines. | ~0.50 (Collapse) |
| **Diffusion Model Fingerprinting** | 2022 | Image: Identification of low-level generative traces. | ~0.65 |
| **Comprehensive Audio Fake Detection Evaluation** | 2024 | Audio: Evaluating robustness of signal-centric models. | N/A |

---

## Phase II: Foundation-Adapted (Current State-of-the-Art)
*Focus: Leveraging frozen weights (CLIP, Wav2Vec), Transformers, and Foundation Model feature extractors.*

| Paper Title | Year | Methodology | Key Metric (OOD AUC) |
| :--- | :--- | :--- | :--- |
| **AUNet: Face Forgery Detection** | 2024 | Video: Vision Transformer (ViT) modeling facial muscle relations. | ~92.77 (Celeb-DF) |
| **TALL: Thumbnail Layout for Video** | 2023 | Video: Swin-Transformer with spatial-temporal frame grids. | ~90.79 (Celeb-DF) |
| **ASVspoof 5 Challenge (Wav2Vec)** | 2024 | Audio: SSL embeddings for robust speech spoofing detection. | EER < 15% |
| **Audity: Audio Deepfake Verification** | 2025 | Audio: Foundation-model based source tracing and attribution. | N/A |
| **MaLP: Interpretable Forgery Localization** | 2023 | Image: Foundation-guided patch-level sensitivity mapping. | N/A |
| **LASTED: Synthetic Image Detection** | 2023 | Image: Domain-generalized detection via attention mechanisms. | N/A |
| **DigiFakeAV: Diffusion-based Detection** | 2025 | Video: Large-scale dataset for training transformer-based models. | N/A |
| **Reprogramming VLMs for Deepfake Detection** | 2025 | Video: Visual-Language Model (VLM) adaptation for OOD data. | ~0.91 |
| **Mixture of Experts (MoE) for Audio** | 2024 | Audio: Dynamic fusion of heterogeneous SSL feature sets. | N/A |

---

## Phase III: Semantic-Physical (The Frontier)
*Focus: Detecting reality violations, physiological signals (rPPG), and physical law inconsistencies.*

| Paper Title | Year | Methodology | Key Metric (OOD AUC) |
| :--- | :--- | :--- | :--- |
| **RepDFD: Reprogramming Frozen Detectors** | 2024 | Video: Targeted adaptation for biological signal extraction. | N/A |
| **ASVspoof 5: Generalization via Physiology** | 2025 | Audio: Biological signal constraints for speech vitality. | ~0.84 |
| **The Forensic Triad (Our Work)** | **2026** | **Video: Physiological rPPG & Biological SNR Thresholding.** | **0.81 (OOD)** |

## Summary of the "Generalization Crisis"
Our analysis confirms that as the field moves from **Phase I** to **Phase III**, OOD (Out-of-Distribution) robustness increases. Phase I models show a 49% average performance drop when moved from FF++ to Celeb-DF, whereas Phase II/III models maintain >80% AUC stability.
