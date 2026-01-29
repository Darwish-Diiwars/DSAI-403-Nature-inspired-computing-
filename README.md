# Metaheuristic Optimization + XAI in NLP  
**DSAI 403 – Nature Inspired Computation**  
Zewail City of Science and Technology

## 📖 Project Overview

This repository contains the code and analysis for the **DSAI 403 final/course project**, demonstrating the application of **nature-inspired metaheuristic algorithms** to multiple stages of an NLP pipeline:

- Hyperparameter tuning of ML/DL models  
- Vocabulary/feature/token selection  
- Optimization of Explainable AI (XAI) methods (especially **LIME** parameters)  
- Meta-optimization (tuning one metaheuristic using another)

We implement and compare **10 unique metaheuristics** across different phases, showing their practical utility in improving model performance and interpretability.

**Key Algorithms Used (10 total)**

| Algorithm                            | Main Phase(s)                  | Primary Purpose                              |
|--------------------------------------|--------------------------------|----------------------------------------------|
| Particle Swarm Optimization (PSO)    | Model Optimization             | Hyperparameter tuning                        |
| Tabu Search                          | Model Optimization             | Hyperparameter tuning                        |
| Simulated Annealing                  | Model Optimization             | Hyperparameter tuning                        |
| Hill Climbing                        | Model Optimization             | Hyperparameter tuning                        |
| Bat Algorithm                        | Model Optimization + XAI       | Hyperparameter + LIME tuning                 |
| Firefly Algorithm                    | Model Optimization             | Hyperparameter tuning                        |
| Ant Colony Optimization (ACO)        | Feature Selection              | Vocabulary/token selection                   |
| Whale Optimization Algorithm (WOA)   | Meta-Optimization + XAI        | Tune Bat/Firefly params + LIME               |
| Grey Wolf Optimizer (GWO)            | XAI Optimization               | LIME parameter optimization                  |
| Cuckoo Search                        | XAI Optimization               | LIME parameter optimization                  |

## ✨ Highlights

- **Comprehensive metaheuristic integration** in a real NLP workflow  
- Usage of swarm intelligence, evolutionary, and trajectory-based methods  
- Optimization at multiple levels: model → features → XAI interpretability  
- Automated summary table generation (`algorithm_usage_summary.csv`)  
- Reproducible Jupyter notebook with full pipeline execution

## 📂 Repository Structure
.
├── DSAI 403 project code .ipynb       ← Main notebook: full pipeline, metaheuristics, XAI, summaries
├── algorithm_usage_summary.csv        ← Generated table (after running notebook)
├── outputs/                           ← (optional) plots, logs, saved models (gitignored if large)
└── README.md

## 🛠️ Requirements

Python 3.10+ / 3.11 recommended

Core libraries used in the notebook (install via pip):

```bash
pip install numpy pandas matplotlib seaborn scikit-learn transformers torch \
    lime shap tqdm requests beautifulsoup4
