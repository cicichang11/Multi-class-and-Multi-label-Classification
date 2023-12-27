# Advanced Analysis of Anuran Calls: Multi-class and Multi-label Classification with SVM and K-Means Clustering

## Overview
This project focuses on the advanced analysis of the Anuran Calls (MFCCs) Dataset, utilizing both classification and clustering techniques. The primary objectives include multi-class and multi-label classification using Support Vector Machines (SVMs) and K-Means clustering. The project explores different SVM approaches, such as Gaussian kernels and L1-penalized SVMs, and addresses class imbalance. It also evaluates classifiers using metrics like exact match and hamming score/loss. Additionally, K-Means clustering is applied to the dataset to understand the majority labels in clusters and to calculate Hamming distance, score, and loss.

## Contents
### 1. Multi-class and Multi-Label Classification Using SVMs
- Data Preparation
- Binary Relevance Approach
- Classifier Evaluation
- L1-Penalized SVMs
- Addressing Class Imbalance
- Classifier Chain Method (Extra Practice)
- Multi-label Classification Metrics (Extra Practice)
- K-Means Clustering on a Multi-Class and Multi-Label Data Set

### 2. Clustering Implementation
- Label Analysis in Clusters
- Hamming Distance Calculation and Monte-Carlo Simulation

## Classification Results
|     | Method                                | Hamming Loss  | Exact Match Ratio  |
|-----|---------------------------------------|---------------|--------------------|
| 0   | Gaussian_SVC_Raw_Attributes           | 0.9856        | 0.0100             |
| 1   | Gaussian_SVC_Standardized_Attributes  | 0.9819        | 0.0117             |
| 2   | L1_Penalized                          | 0.9231        | 0.0513             |
| 3   | SMOTE                                 | 0.868         | 0.0684             |


## Clustering Results
|     | Avg Hamming Distance | Std of Hamming Distance | Avg Hamming Loss | Std of Hamming Loss | Avg Hamming Score | Std of Hamming Score |
|-----|----------------------|-------------------------|------------------|---------------------|-------------------|--------------------------|
| 0   | 0.6614               | 0.027                   | 0.2205           | 0.009	              | 0.7795	          | 0.009                    |

## Dependencies
- Python 3.x
- Pandas
- Scikit-Learn
- Seaborn
- Matplotlib
- Numpy
- Imbalanced-Learn

## Installation
Clone the repository and install the required Python packages.
```bash
git clone [repository-url]
pip install -r requirements.txt
```

## Usage
Run the Jupyter Notebook to reproduce the results:
```bash
jupyter notebook Multi-class_and_Multi-label_Classification.ipynb
```
