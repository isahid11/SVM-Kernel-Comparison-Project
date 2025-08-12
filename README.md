# SVM-Kernel-Comparison-Project

## Overview
This project evaluates **Support Vector Machine (SVM)** classifiers across three kernels — **Linear**, **RBF**, and **Polynomial** — with hyperparameter tuning (`C` parameter) and performance comparison. The aim is to determine which kernel performs best for the given datasets.

## Datasets
- **Bank Marketing Dataset**: Predicts whether a client will subscribe to a term deposit.  
  [https://archive.ics.uci.edu/dataset/222/bank+marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing)

- **Electrical Grid Stability Dataset**: Classifies electrical grid stability conditions.  
  [https://archive.ics.uci.edu/dataset/471/electrical+grid+stability+simulated+data](https://archive.ics.uci.edu/dataset/471/electrical+grid+stability+simulated+data)

## Workflow
1. **Load & Preprocess Data**: Applied one-hot encoding, feature scaling, and train-test splitting.
2. **Model Training**: Implemented SVM models with Linear, RBF, and Polynomial kernels.
3. **Hyperparameter Tuning**: Used GridSearchCV to optimize the `C` parameter for each kernel.
4. **Evaluation**: Assessed accuracy, precision, recall, and F1-score.
5. **Comparison**: Summarized and compared model performance.

## Results Summary

| Kernel       | Best C | Accuracy |
|--------------|--------|----------|
| Linear       | 100    | 99.8%    |
| RBF          | 1      | 98.15%   |
| Polynomial   | 10     | 96.9%    |

> **Insight:** The Linear kernel achieved the highest accuracy with simpler computation, making it the best-performing option for these datasets.
