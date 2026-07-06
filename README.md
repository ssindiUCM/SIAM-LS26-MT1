# Interpretable Machine Learning and Deep Learning for Biological Modeling

**SIAM Life Sciences 2026 — Minitutorial #1**  
Monday, July 6 · 8:00–10:00 AM · Grand Ballroom C

---

## Overview

Biological data analysis increasingly relies on machine learning, yet balancing predictive accuracy with interpretability remains a key challenge. This mini-tutorial provides a practical introduction to machine learning approaches in biological modeling, from classical machine learning to deep learning.

We begin with foundational concepts — including the trade-off between accuracy and interpretability, and challenges posed by small, noisy datasets common in biological research. We then demonstrate workflows for representative methods such as linear models, symbolic regression, and deep learning using synthetic and real biological datasets. By the end, attendees will be familiar with key workflows and considerations for applying interpretable machine learning and deep learning in biological modeling.

**Learning Objectives**

*Part 1: Traditional Machine Learning*
- Understand the interpretability–accuracy trade-off
- Select appropriate ML methods for biological data
- Recognize and avoid common pitfalls in biological modeling

*Part 2: Deep Learning*
- Understand the core language of deep learning
- Understand the interpretability spectrum within deep learning
- See where deep learning meets mechanistic modeling

---

## Schedule

| Time | Topic |
|------|-------|
| 10 min | Overview & Orientation |
| 50 min | Traditional Machine Learning — definitions, classification, interpretability |
| 50 min | Deep Learning — definitions, image classification, BINNs for ODE parameter recovery |
| 10 min | Wrap-Up |

---

## Slides

| Format | Link |
|--------|------|
| PDF | [MT1-Slides.pdf](MT1-Slides.pdf) |
| Google Slides | [View online](https://docs.google.com/presentation/d/1FqeB20gf3gtZ1KJ6O0laSp-UuNLFPMbBN8Y90BVH7zg/edit?usp=sharing) |

---

## Notebooks

All examples are implemented as Jupyter notebooks designed to run in Google Colab.

| Notebook | Topic |
|----------|-------|
| `ML_Example1_Classification.ipynb` | Traditional ML: logistic regression, interpretability trade-offs |
| `ML_Example2_BreastCancer.ipynb` | Traditional ML: application of ML methods to breast cancer data |
| `DL_Example0_LogisticRegression.ipynb` | Bridge: logistic regression = single neuron; scikit-learn vs. TensorFlow |
| `DL_Example1_MNIST_to_PneumoniaMNIST.ipynb` | Deep Learning: image classification with MLPs and CNNs; Grad-CAM interpretability |
| `DL_Example2_BINNs.ipynb` | BINNs: biologically-informed neural networks for ODE parameter recovery |

### Data

| File | Description |
|------|-------------|
| `data/lynx_hare.csv` | Hudson Bay lynx–hare population time series (1900–1920) used in `DL_Example2_BINNs.ipynb` |

---

## Getting Started

You can run all notebooks directly in your browser using [Google Colab](https://colab.research.google.com/) — no installation required.

**Requirements:** a Google account and internet access.

### Option 1: Open directly in Colab

Click any notebook in this repository, then click the **"Open in Colab"** badge or button at the top of the file.

### Option 2: Clone to your Google Drive

Run these cells at the top of a Colab notebook:

```python
from google.colab import drive
drive.mount('/content/drive')

%cd /content/drive/MyDrive/
!git clone https://github.com/ssindiUCM/SIAM-LS26-MT1
%cd SIAM-LS26-MT1
```

### Option 3: Run locally

```bash
git clone https://github.com/ssindiUCM/SIAM-LS26-MT1
cd SIAM-LS26-MT1
pip install numpy matplotlib scikit-learn tensorflow
jupyter notebook
```

---

## Organizers

**Suzanne Fernandes-Sindi** — University of California, Merced  
**Tracey Oellerich** — University of North Carolina, Chapel Hill

---

## Citation / Acknowledgment

If you use these materials, please acknowledge:

> Sindi, S. and Oellerich, T. *Interpretable Machine Learning and Deep Learning for Biological Modeling.* SIAM Life Sciences Minitutorial, July 2026.

---

## License

This repository is shared for educational use. See [LICENSE](LICENSE) for details.
