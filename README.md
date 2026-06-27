# Forecasting Precipitation in Cuba Using Graph Neural Networks

## Overview

This repository contains my master's research project on daily precipitation forecasting in Cuba using Graph Neural Networks and Long Short-Term Memory (LSTM) models.

The objective of this work is to investigate how incorporating spatial relationships between weather stations improves precipitation prediction compared with conventional temporal deep learning models.

Three deep learning models are evaluated:

* Graph Convolutional Recurrent Neural Network (GCRNN)
* Partially Masked LSTM
* Masked LSTM

Model performance is evaluated using eight held-out test nodes from NOAA CPC Unified daily precipitation observations.

---

## Dataset

* **Source:** NOAA CPC Unified Daily Precipitation Dataset
* **Study Area:** Cuba
* **Time Period:** 1979–2023
* **Prediction Horizon:** Daily precipitation forecasting
* **Evaluation:** Eight unseen (held-out) test nodes

---

## Models

### GCRNN

A Graph Convolutional Recurrent Neural Network designed to capture both temporal rainfall dynamics and spatial relationships among neighboring locations.

### Partially Masked LSTM

An LSTM model that incorporates limited neighborhood information together with temporal observations.

### Masked LSTM

A baseline LSTM model that relies only on temporal information without explicit spatial connectivity.

---

## Repository Structure

```text
precipitation-forecasting-cuba/
│
├── README.md
├── requirements.txt
├── Masked LSTM-Partially Masked LSTM-GCRNN.ipynb
├── Cuba_Precipitation_with_Nodes 3(in).csv
├── cuba_node_edges.csv
│
└── figures/
    ├── gcrnn/
    ├── masked_lstm/
    └── partially_masked_lstm/

## Installation

Clone the repository and install the required packages:

```bash
pip install -r requirements.txt
```

---

## Figures

The **figures** directory contains representative prediction results for the eight held-out test nodes.

Each model includes:

* Timeline prediction plots
* Test scatter plots
* Comparison of observed versus predicted precipitation

---

## Requirements

Install the required Python packages using:

```bash
pip install -r requirements.txt
```

---

## Main Python Libraries

* NumPy
* Pandas
* Matplotlib
* SciPy
* NetworkX
* PyTorch
* TensorFlow
* Scikit-learn
* Optuna
* Jupyter Notebook

---

## Author

**Taufiqul Islam**

M.S. Earth & Environmental Sciences

The University of Texas at Arlington
