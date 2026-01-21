<img width="1480" height="480" alt="ChatGPT Image Jan 21, 2026, 11_53_33 AM" src="https://github.com/user-attachments/assets/8c8a6624-3377-4f18-8f0d-accb85a9afff" />

🚧 **Work in Progress**  
This repository represents an **active, evolving research project**. Notebooks, models, and results are **not final** and will change as the project progresses toward a broader clinical AI system.

## Vision & Final Goal

This project is a foundational component of a **cardiology-focused AI system** that goes **beyond traditional Retrieval-Augmented Generation (RAG)**.

The long-term goal is to build an **AI cardiology assistant** that integrates:

- **Fine-tuned Large Language Models (LLMs)** capable of reasoning like a cardiologist
- **ECG deep learning models** for rhythm disorders and ischemia detection
- **Imaging models for echocardiography interpretation**
- **Risk prediction models** for established cardiac scores and outcomes
- **Guideline-grounded RAG** for decision-making support with:
    - ACC/AHA guidelines
    - ESC guidelines

This repository focuses specifically on the **ECG intelligence layer**, starting with **PTB-XL**.

## Current Scope (This Repository)

The repository focuses on:

- **Automatic ECG diagnosis** using the **PTB-XL dataset**
- **Multi-label classification** for ECG recordings, as an ECG may show multiple conditions simultaneously
- **Learning diagnostic patterns** directly from raw ECG waveforms
- Establishing a reliable **ECG modeling baseline** for downstream clinical reasoning

The outputs of this project will **feed into higher-level reasoning models**, rather than serve as a standalone diagnostic system.

## Dataset

**PTB-XL (version 1.0.3)**  
A large, publicly available dataset of clinical 12-lead ECG recordings:

- **21,799 ECG recordings**
- **12 leads**, 10 seconds each
- Sampling rates: **100 Hz** and **500 Hz**
- **Expert annotations** using **SCP-ECG diagnostic statements**

### Diagnostic Superclasses:

- **NORM**: Normal ECG
- **MI**: Myocardial Infarction
- **STTC**: ST/T Wave Changes
- **CD**: Conduction Disturbances
- **HYP**: Hypertrophy

This dataset is used to approach the **multi-label classification problem**. ECG signals often exhibit multiple conditions simultaneously.

## Methodology

The project will employ the following approaches:

- **Signal preprocessing** and **quality assessment**
- **Deep learning models** applied directly to raw ECG signals, including:
    - CNN-based architectures
    - Sequence models (LSTM, GRU)
- **Patient-aware, stratified data splits** for validation
- **Model interpretability** to ensure clinical relevance

The integration of **multimodal data** (e.g., echocardiography, clinical context) and **advanced reasoning models** will be prioritized in later stages.

## Planned Repository Structure

```plaintext
AI-Assisted-ECG-Diagnosis/
├── notebooks/          # Data understanding, EDA, modeling
├── data/              # Dataset access scripts (raw data not included)
├── models/            # Trained models and checkpoints
├── utils/             # Preprocessing and helper functions
├── docs/              # Project notes and design decisions
└── README.md          # Project documentation
```

## Current Progress

- **✔️** Data understanding and target definition
- **✔️** Analysis of ECG-related physiological factors
- **🔄** Signal preprocessing and quality checks
- **🔄** Baseline model development
- **⏳** Advanced modeling and evaluation
- **⏳** Integration planning with higher-level clinical AI components

## Planned Tools & Libraries

- **Python 3.9+**
- **NumPy**, **Pandas**, **SciPy**
- **scikit-learn**
- **TensorFlow** or **PyTorch**
- **WFDB** (ECG signal handling)

A `requirements.txt` file will be provided later.

## Important Notes

- This project is for **research and educational purposes only**.
- The **PTB-XL dataset** must be downloaded separately from **PhysioNet** and is subject to its data usage agreement.
- The outputs from this repository **are not clinically validated** and must not be used for medical decision-making.

## Acknowledgments

- **PhysioNet** for hosting the PTB-XL dataset
- The **PTB-XL authors** for creating and documenting the dataset
- Open-source contributors in the **ECG** and **medical AI** communities

## Long-Term Outlook

This repository represents the **ECG foundation** of a larger **clinical AI system** aimed at:

> **Combining multimodal cardiac data with guideline-aware reasoning to support cardiology decision-making.**
