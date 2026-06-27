# Forecasting Precipitation in Cuba Using Graph Neural Networks

## Overview

This repository presents my master's research on daily precipitation forecasting in Cuba using graph-based deep learning and LSTM models.

The project compares three models:

- Graph Convolutional Recurrent Neural Network (GCRNN)
- Partially Masked LSTM
- Masked LSTM

The goal was to evaluate how well these models predict precipitation at held-out test nodes using NOAA CPC Unified daily precipitation observations.

## Dataset

- Source: NOAA CPC Unified Daily Precipitation
- Study area: Cuba
- Time period: 1979–2023
- Evaluation focus: eight held-out test nodes

## Models

### GCRNN
Graph-based model designed to capture both temporal rainfall patterns and spatial relationships between nodes.

### Partially Masked LSTM
LSTM model using partial spatial/neighborhood information.

### Masked LSTM
Baseline LSTM model using temporal information only.

## Repository Structure

```text
precipitation-forecasting-cuba/
│
├── README.md
├── requirements.txt
├── Masked LSTM-Partially Masked LSTM-GCRNN.ipynb
├── Cuba_Precipitation_with_Nodes 3(in).csv
├── cuba_node_edges.csv
└── figures/
    ├── gcrnn/
    ├── masked_lstm/
    └── partially_masked_lstm/
