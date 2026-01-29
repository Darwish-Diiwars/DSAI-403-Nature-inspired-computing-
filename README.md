# Nature-Inspired Computation – DSAI 403 Final Project  
**Metaheuristic Optimization for Deep Learning & Explainable AI in NLP**

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)  
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)](https://www.tensorflow.org/)  
[![License: Educational](https://img.shields.io/badge/License-Educational-yellow)](LICENSE)

Zewail City of Science and Technology – DSAI 403: Nature Inspired Computation  
**December 2025**

## 🎯 Project Overview

This project demonstrates the power of **nature-inspired metaheuristic algorithms** in optimizing a complete NLP pipeline:

- **Model**: Bidirectional GRU with BERT tokenization  
- **Task**: Multi-class sentiment classification (1–5 stars)  
- **Dataset**: TripAdvisor Hotel Reviews (~7,000 samples)  
- **Main Goal**: Improve model performance + enhance explainability using **10 unique metaheuristics**

We apply swarm intelligence, evolutionary, and trajectory-based methods across **three optimization levels**:

1. Model hyperparameter tuning  
2. Vocabulary/feature selection  
3. LIME (Local Interpretable Model-agnostic Explanations) parameter optimization  
4. Meta-optimization (tuning hyperparameters of other metaheuristics)

## 🧬 Algorithms Implemented (10 Unique)

| #  | Algorithm                        | Phase                              | Purpose                                      |
|----|----------------------------------|------------------------------------|----------------------------------------------|
| 1  | Particle Swarm Optimization (PSO) | Model Optimization                 | Hyperparameter tuning                        |
| 2  | Tabu Search                      | Model Optimization                 | Hyperparameter tuning                        |
| 3  | Simulated Annealing              | Model Optimization                 | Hyperparameter tuning                        |
| 4  | Hill Climbing                    | Model Optimization                 | Hyperparameter tuning                        |
| 5  | Bat Algorithm                    | Model Optimization + XAI           | Hyperparameter + LIME tuning                 |
| 6  | Firefly Algorithm                | Model Optimization                 | Hyperparameter tuning                        |
| 7  | Ant Colony Optimization (ACO)    | Feature Selection                  | Vocabulary / token selection                 |
| 8  | Whale Optimization Algorithm (WOA) | Meta-Optimization + XAI          | Tunes Bat & Firefly parameters + LIME        |
| 9  | Grey Wolf Optimizer (GWO)        | XAI Optimization                   | LIME parameter optimization                  |
| 10 | Cuckoo Search                    | XAI Optimization                   | LIME parameter optimization                  |

## 📈 Key Results

### Model Performance Comparison

| Method                | Validation Loss | Validation Accuracy | Improvement over Baseline |
|-----------------------|-----------------|----------------------|----------------------------|
| **Baseline**          | 1.2997          | 43.88%              | —                          |
| PSO                   | 1.1089          | 52.48%              | +19.60%                    |
| Tabu Search           | 1.1147          | 48.57%              | +10.70%                    |
| Simulated Annealing   | 1.4321          | 49.24%              | +12.22%                    |
| Hill Climbing         | 1.2132          | 52.57%              | +19.81%                    |
| **Bat Algorithm**     | **1.0586**      | 50.48%              | +15.04%                    |
| Firefly Algorithm     | —               | —                   | —                          |

**Best improvement**: **+19.81% accuracy** (Hill Climbing)  
**Best loss reduction**: **~18.6%** (Bat Algorithm)

### XAI (LIME) Optimization Results

| Algorithm | # of Samples | # of Features | Fidelity Score |
|-----------|--------------|---------------|----------------|
| GWO       | 715          | 11            | 0.0978         |
| Bat       | 1,010        | 13            | 0.1798         |
| **WOA**   | **531**      | **15**        | **0.2057**     |
| Cuckoo    | 845          | 9             | 0.1656         |

**Best fidelity score**: **0.2057** (Whale Optimization Algorithm)

## 🏆 Main Achievements

- **+19.81%** accuracy improvement over baseline  
- **~18.6%** reduction in validation loss  
- Successfully implemented **meta-optimization** (WOA tuning Bat & Firefly parameters)  
- Optimized **LIME explainability** reaching **0.2057 fidelity score**  
- Applied **10 different nature-inspired algorithms** in a coherent pipeline  
- Demonstrated real-world applicability of swarm intelligence in deep learning & XAI

## 📁 Project Structure
NIC-DSAI403-Final/
├── nic-local-host-1-1 (5).ipynb      # Main notebook – full pipeline & experiments
├── algorithm_usage_summary.csv       # Summary table of all 10 algorithms (auto-generated)
├── report.tex                        # Full LaTeX project report
├── report.pdf                        # (optional) Compiled report
├── *.csv                             # Generated results & logs
└── README.md                         # This file

## 📚 Requirements

Python 3.8+
TensorFlow 2.x
PyTorch
transformers (Hugging Face)
pyswarms
lime
numpy, pandas, matplotlib, seaborn, scikit-learn, tqdm

## 🔗 References (selected)

Kennedy, J., & Eberhart, R. (1995). Particle swarm optimization
Dorigo, M., & Stützle, T. (2004). Ant Colony Optimization
Mirjalili, S., & Lewis, A. (2016). The whale optimization algorithm
Yang, X. S. (2010). A new metaheuristic bat-inspired algorithm
Yang, X. S. (2009). Firefly algorithms for multimodal optimization
Mirjalili, S. et al. (2014). Grey wolf optimizer
Ribeiro, M. T. et al. (2016). "Why should I trust you?": Explaining the predictions of any classifier (LIME)

## 📝 License
Educational / Academic use only.
This project is part of the DSAI 403 – Nature Inspired Computation course at Zewail City.
Made with 🐺🦅🦇🔥🐳 for DSAI 403 – December 2025
