# Sentinel: A White-Box Ensemble Framework for Explainable Deepfake Detection

**Sentinel** is an advanced forensic auditing tool designed to move beyond "Black-Box" AI detection. By synthesizing neural texture analysis, spectral frequency fingerprints, and 3D geometric consistency, Sentinel provides a verifiable forensic report for digital media investigations.

## Key Features

* **Multi-Pillar Forensic Audit**:
    * **Neural Engine**: Backbone utilizing **MobileNetV2** for localized artifact and texture-level assessment.
    * **Spectral Pillar**: Employs **Fast Fourier Transform (FFT)** to expose "checkerboard" up-sampling artifacts invisible to the human eye.
    * **Geometric Pillar**: Analyzes the **"Perspective Paradox"**—detecting misalignments between 3D facial landmarks and 2D texture depth.
* **The Veto Step (Core Novelty)**: A deterministic rule-based priority engine. If a physical geometric impossibility is detected, the system triggers a **Geometric Veto**, overriding neural uncertainty with immutable physical laws.
* **White-Box Interpretability**: Provides **1D Power Spectrum (Radial Average)** graphs and 3D landmark maps to justify every verdict with mathematical and physical proof.
* **Forensic Analyst Suite**: A professional-grade UI built with **Gradio** for real-time image auditing and analyst feedback loops.

## Methodology

Sentinel utilizes the **Synthetic Reliability Index (SRI)** to aggregate findings:
1.  **Frequency Analysis**: $LogSpectrum = 20 \cdot \log(|FFT(Image)| + 1)$ targets generative model fingerprints.
2.  **Geometric Consistency**: Evaluates 3D landmark ratios to identify structural flaws in AI generation.
3.  **Decision Fusion**: Combines weighted neural scores with a hard veto override for physical paradoxes.

## Datasets

The system is trained and validated using:
* **FFHQ (Flickr-Faces-HQ)**: Authentic high-resolution facial baseline.
* **GenAI Dataset**: Comprehensive synthetic face collection.
* **CIFAKE**: Benchmark for explainable identification performance.

## Usage

```bash
# Install dependencies
pip install -r requirements.txt
