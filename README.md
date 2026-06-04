### Applied Machine Learning for Clinical Prediction
**Palm Spring · 2026**

> A hands-on machine learning workshop using real clinical data from the University of Wisconsin Breast Cancer Diagnostic dataset. Participants build a complete ML pipeline from raw data to a live patient prediction in 90 minutes, entirely in Google Colab.

---

## 👥 Credits

| Role | Name |
|------|------|
| **Created by** | Berna Alemdag |
| **Academic Advisors** | Dr. Gözde Kabay · Prof. Matthias Franzreb|
| **Department** | BEBS |

---

## 📋 Workshop Overview

| Property | Detail |
|----------|--------|
| **Duration** | 90 minutes |
| **Platform** | Google Colab no installation required |
| **Dataset** | Wisconsin Breast Cancer Diagnostic (UCI ML Repository) |
| **Model** | Random Forest Classifier |
| **Audience** | Beginners |
| **Tasks** | 7 hands-on participant tasks |

---

## 🗺️ Workshop Roadmap

| Block | Topic | Format |
|-------|-------|--------|
| Block 0 | Environment setup | Task |
| Block 1 | Data acquisition from UCI | Task |
| Block 2 | Class distribution analysis | Task |
| Block 3 | Correlation heatmap and feature reduction | Task |
| Block 4 | Random Forest full ML pipeline | Demo + 2 Tasks |
| Block 5 | SHAP explainability analysis | Demo |
| Block 6 | Save model | Demo |
| Block 7 | Live prediction of new patient diagnosis | Task |

---

## 🚀 Quick Start

### Option 1 - Open directly in Google Colab (recommended)

Click the badge below to open the notebook instantly:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BernaAlemdag/palmspring-ml-workshop-2026/blob/main/PalmSpringWS12026.ipynb)

> **Before you start:**
> 1. Click the badge above to open the notebook in Google Colab
> 2. Go to **File → Save a copy in Drive**
> 3. Rename your copy to `PalmSpringWS12026_YOURNAME` (e.g. `PalmSpringWS2026_Anna`)
> 4. Work in your own copy, do not edit the original

### Option 2 - Clone and run locally

```bash
git clone https://github.com/BernaAlemdag/palmspring-ml-workshop-2026.git
cd palmspring-ml-workshop-2026
pip install -r requirements.txt
jupyter notebook PalmSpringWS12026.ipynb
```

---

## 📁 Repository Structure

```
diagnosis-by-data/
│
├── berna_PalmspringWS2026.ipynb     # Main workshop notebook
├── README.md                         # This file
├── LICENSE                           # License

```

---



| Library | Version | Purpose |
|---------|---------|---------|
| `numpy` | ≥ 1.24 | Numerical computation |
| `pandas` | ≥ 2.0 | Data manipulation |
| `matplotlib` | ≥ 3.7 | Plotting |
| `seaborn` | ≥ 0.12 | Statistical visualisation |
| `scikit-learn` | ≥ 1.3 | ML models and evaluation |
| `shap` | ≥ 0.43 | Explainability analysis |
| `ucimlrepo` | ≥ 0.0.3 | UCI dataset API |

---

## 🧬 The Dataset

We use the **Wisconsin Breast Cancer Diagnostic (WBCD) dataset**,
first described by Street, Wolberg & Mangasarian (1993).

| Property | Detail |
|----------|--------|
| Samples | 569 patients |
| Features | 30 continuous measurements |
| Source | Digitised FNA cell nucleus images |
| Target | Malignant (M) or Benign (B) |
| Missing values | None |

The dataset is fetched directly from the UCI ML Repository at runtime — no manual download required.

> UCI page: https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic

---

## 🎯 Learning Outcomes

By the end of this workshop, participants will be able to:

- Load and inspect a real clinical dataset from a public research archive
- Identify and remove redundant features using correlation analysis
- Train a Random Forest classifier and evaluate it with clinical metrics
- Interpret Accuracy, Precision, Recall, and F1-score in a medical context
- Run K-fold cross-validation and assess model stability
- Understand SHAP explainability and why it matters in clinical AI
- Save a trained model and perform a live patient prediction

---

## 📊 What Participants Build

```
Raw patient data (569 patients, 30 features)
        ↓
Correlation analysis → Feature reduction (30 → ~20 features)
        ↓
80/20 train/test split
        ↓
Random Forest Classifier (100 trees)
        ↓
Evaluation: Accuracy, Precision, Recall, F1
        ↓
Cross-validation: K = 3, 5, 7 stability analysis
        ↓
SHAP explainability analysis
        ↓
Saved model → Live prediction of new patient diagnosis
```

---

## ✏️ Participant Tasks

| Task | What they do |
|------|-------------|
| Task 0 | Import 3 libraries with correct aliases |
| Task 1 | Fetch the dataset directly from the UCI page |
| Task 2 | Reproduce the class distribution chart with custom colours |
| Task 3 | Apply correlation filter (τ = 0.90) and redraw the heatmap |
| Task 4a | Experiment with different split ratios and tree counts |
| Task 4b | Compare 3-fold and 7-fold cross-validation stability |
| Task 7 | Enter patient measurements and run a live prediction |

---

---

## ⚠️ Ethical Declaration

All analyses in this workshop are conducted for **educational purposes exclusively**.
No output constitutes a clinical recommendation or medical advice.

Deployment of any ML model in a diagnostic context requires:
- Prospective clinical validation across multiple institutions
- Peer-reviewed publication of results
- Regulatory clearance (e.g. FDA 510(k) or EU MDR)
- Institutional ethics approval and ongoing post-deployment monitoring



---

## 🙏 Acknowledgements

- **Dataset:** Wolberg, W., Street, W., & Mangasarian, O. (1993). *Wisconsin Breast Cancer Diagnostic Dataset*. UCI Machine Learning Repository.
- **SHAP:** Lundberg, S. M., & Lee, S. I. (2017). *A Unified Approach to Interpreting Model Predictions*. NeurIPS.

---

*Applied Machine Learning for Clinical Prediction · Palm Springs 2026*
