# On the Geometry of Truthfulness: Interpretable Steering in Representation Space

**Course:** Deep Generative Models - Winter 1404  
**Status:** In Progress / Proposal Phase

## 📄 Project Overview

This repository contains the codebase and research proposal for our investigation into the geometry of truthfulness in Large Language Models (LLMs). 

### Abstract
Recent advancements in LLM interpretability have introduced "steering vectors"—linear directions in activation space that can control model behavior. However, current methods largely rely on the unverified assumption of a "universal correction vector" that can transform any hallucinated state into a truthful one.

Our research challenges this assumption. We argue that truthfulness is not a fixed direction but a complex distribution. We propose shifting from vector-based steering to **Distributional Learning**, using generative models to map the distribution of hallucinated representations onto truthful ones, thereby capturing the underlying geometry of truthfulness more faithfully.

## 📂 Repository Structure

To keep our work organized, we are using the following directory structure. Please place files in their respective folders:

```text
├── proposal/              # LaTeX source files and PDF of the project proposal
│   ├── main.tex
│   ├── references.bib
│   ├── figures/
│   └── proposal.pdf       # Compiled proposal
├── src/                   # Source code for the project
│   ├── data/              # Data loading and preprocessing scripts
│   ├── models/            # Model definitions (Steering vectors, Generative mappers)
│   ├── analysis/          # Code for PCA, KDE, and geometry visualization
│   └── utils/             # Helper functions
├── experiments/           # Scripts to run specific experiments
├── notebooks/             # Jupyter notebooks for exploration and visualization
├── results/               # Generated figures and logs
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation
```

## 🎯 Research Objectives

Building on the critique of the "Universal Correction Vector," this project aims to address the following research questions:

1.  **Validity Check:** Is the assumption of a universal truthful direction in the activation space of LLMs theoretically grounded and empirically valid?
2.  **Modeling:** How can distributional learning frameworks model the transformation from hallucinated to truthful representations?
3.  **Structure:** What projection or decomposition methods best capture the underlying structure of hidden state distributions?
4.  **Global vs. Local:** Does a single global direction consistently move hallucinated activations toward truthful ones across diverse domains, or are multiple localized sub-vectors more effective?

## 🛠️ Getting Started

### Prerequisites
*   Python 3.8+
*   PyTorch
*   Transformers (HuggingFace)

### Installation
(To be updated as code is added)
```bash
git clone https://github.com/your-username/geometry-of-truthfulness.git
cd geometry-of-truthfulness
pip install -r requirements.txt
```

## 📝 Proposal Access

The detailed theoretical background and mathematical formulation are available in the project proposal.
*   **[View PDF Proposal](./proposal/proposal.pdf)** (Ensure you compile the latex or upload the PDF to this path)
*   **LaTeX Source:** Located in the `proposal/` directory.

## 📚 References

This project references the following key works:

*   **Cao et al. (2024)**: *Personalized steering of large language models: Versatile steering vectors through bi-directional preference optimization.* [arXiv](https://arxiv.org/abs/2406.00045)
*   **Chen et al. (2024)**: *Truth forest: Toward multi-scale truthfulness in large language models through intervention without tuning.* AAAI Conference on Artificial Intelligence.
*   **Li et al. (2024)**: *Inference-time intervention: Eliciting truthful answers from a language model.* [arXiv](https://arxiv.org/abs/2306.03341)
*   **Wang et al. (2025)**: *Truthflow: Truthful LLM generation via representation flow correction.* [arXiv](https://arxiv.org/abs/2502.04556)

---
*Maintained by the Research Team for Deep Generative Models (Winter 1404).*
```
