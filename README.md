# 3-Layer-EEG-Conformer-Network

Official project repository for the advanced deep learning framework engineered for highly resilient Motor Imagery decoding.

## 📌 Project Overview
This repository contains the architecture and implementation code for an advanced 3-layer Conformer network framework. Designed specifically for Electroencephalogram (EEG) signals, this network combines the local feature-extraction capabilities of Convolutional Neural Networks (CNNs) with the global context-awareness of Transformers to achieve high-accuracy biosignal classification.

By systematically replacing redundant multi-branch parallel configurations with a strictly serialized spatiotemporal shallow feature pipeline and a sequential 3-layer transformer encoder cascade, this framework eliminates parameter bloating and prevents numerical saturation across continuous execution runs.

### Key Features:
* **3-Layer Serialized Conformer Core:** Optimized for serialized temporal-spatial modeling of stochastic brainwaves without parallel redundancy.
* **End-to-End Pipeline:** Preprocessing, bandpass filtering, robust scaling normalization, and training logic.
* **Robust Performance:** Achieved state-of-the-art accuracies of **88.33%** on Dataset 2a and **92.46%** on Dataset 2b under strict Subject-Isolated Cross-Validation.

---

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Frameworks:** PyTorch
* **Libraries:** MNE-Python, NumPy, Scikit-learn, Matplotlib
* **Target Dataset:** BCI Competition IV Dataset 2a & BCI Competition IV Dataset 2b

---

## 📂 Repository Structure
* `/models` — Neural network architecture files (serialized spatiotemporal blocks and conformer layers).
* `/preprocessing` — Signal conditioning, zero-phase bandpass filtering, and epoch segmentation scripts.
* `train.py` — Main model training, optimization trajectories, and subject-isolated validation pipeline.
* `.gitignore` — Standard Python environment file exclusions.
