# protector-v2
# Protector v2 — Multi-Agent AI Security System

[![Python](https://img.shields.io/badge/Python-3.10+-blue)](https://python.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)](https://tensorflow.org)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Kaggle](https://img.shields.io/badge/Kaggle-Notebooks-blue)](https://kaggle.com)

## What is Protector v2?

A production-grade, real-time AI security system that runs 14 ML/DL agents
simultaneously on your local machine, detecting intrusions and malware across
3 research datasets with SHAP explainability and attack family classification.

## Architecture

![Architecture](assets/architecture.png)

## Notebooks

| # | Notebook | Dataset | Purpose |
|---|----------|---------|---------|
| 1 | [NB1 — Classical ML](nb1_classical_ml/) | CIC-IDS 2018 | SVM, RF, NB, ELM, Ensemble |
| 2 | [NB2 — Deep Learning](nb2_deep_learning/) | UNSW-NB15 | CNN, LSTM, GRU, ResNet, GAN |
| 3 | [NB3 — Advanced](nb3_advanced/) | BETH | HMM, HDBSCAN, Process2Vec |
| 4 | [NB4 — i3 Endpoint](nb4_endpoint/) | Live system | 14-agent fusion, tray, dashboard |
| 5 | [NB5 — Explainability](nb5_explainability/) | CIC-IDS 2018 | SHAP, GradCAM, Family CLF |

## Results

| Model | Dataset | Accuracy | Notes |
|-------|---------|----------|-------|
| Random Forest | CIC-IDS 2018 | ~97% | Multi-class, 5 attack types |
| ResNet-1D | UNSW-NB15 | ~96% | Binary sequence detection |
| HDBSCAN | BETH | — | Unsupervised cluster discovery |
| SHAP Explainer | CIC-IDS 2018 | — | Top feature: Flow Duration |
| Meta Ensemble | CIC-IDS 2018 | ~98% | Stacked LR on 5 base models |

## Quick Start

# Clone
git clone https://github.com/YOUR_USERNAME/protector-v2.git
cd protector-v2

# Install
pip install -r nb4_endpoint/requirements.txt

# Run endpoint (after downloading models from Kaggle)
cd nb4_endpoint
python tray.py

## Screenshots

Dashboard | SHAP | NetworkX Graph  
