
```markdown
# 🧠 Multi-Modal Alzheimer’s Disease Diagnosis using Multi-Scale Graph Neural Networks

This repository contains the implementation of our research project:  
**"A Multi-Scale Graph Neural Network for Early Diagnosis of Alzheimer’s Disease using Genomic, Proteomic, and Neuroimaging Data."**

 📌 Overview

Alzheimer’s Disease (AD) is a complex neurodegenerative disorder. This project proposes a novel **multi-scale Graph Neural Network (GNN)** framework that integrates **genomic**, **proteomic**, and **neuroimaging** data to improve early detection and interpretation of AD.

 🧬 Key Features
- Multi-modal data fusion: Gene expression, protein-protein interaction, and brain connectivity
- Layered graph construction per modality
- Attention mechanisms for improved interpretability
- Evaluation on benchmark Alzheimer’s datasets
- Model capable of discovering biologically meaningful patterns

---
```

 🚀 Getting Started

# Prerequisites

- Python 3.8+
- PyTorch
- PyTorch Geometric
- NumPy, pandas, matplotlib
- scikit-learn

# Installation

```bash
git clone https://github.com/spk-22/Neuro-Fusion.git
python ad_gnn.py
```



 📊 Datasets

We used publicly available datasets such as:

* **ADNI (Alzheimer’s Disease Neuroimaging Initiative)** for neuroimaging
* **GEO** or **TCGA** for genomic/proteomic data
---

 🧠 Model Architecture

* Each modality (genomic, proteomic, neuroimaging) is represented as a graph.
* Graph convolution layers are applied to each.
* A cross-modal attention mechanism is used to integrate features.
* The combined features are passed through an MLP for classification (AD vs CN vs MCI).

---

 📈 Results

| Metric          | Accuracy | F1-Score | Control AUC  |  Early AD | Late AD |
| --------------- | -------- | -------- | -------------|-----------|---------|
| Multi-Modal GNN |  98.00%  |  0.9800  |     0.98     |    0.98   |   1.00  |

---

  Acknowledgements

* Alzheimer's Disease Neuroimaging Initiative (ADNI)
* GEO, TCGA for genomic and proteomic data
* PyTorch Geometric for GNN implementation
