# Data-Mining-UNAM

## Overview
This repository contains several projects from the Data Mining course at UNAM, Mexico. These projects were developed throughout the semester 24-2, with each one being presented and detailed extensively. The aim of these projects is to extract valuable insights from various datasets relevant to customer behavior, sales transactions, and text generation based on the Harry Potter series.

---

## Project Structure

### [1. Sales Beverage](https://github.com/haroldeustaquio/Data-Mining-UNAM/tree/main/sales-beverage)

#### Overview
The Sales Beverage project analyzes transaction data for isotonic drinks, utilizing association and time series models to identify purchasing patterns and trends in customer behavior. The ultimate goal is to enhance marketing and sales strategies for beverage companies.

#### Models Applied
1. [Association Models](https://github.com/haroldeustaquio/Data-Mining-UNAM/blob/main/sales-beverage/association.ipynb) :
   - **``Apriori``**: Finds frequent relationships between purchased products.
   - **``FP-Growth``**: Improves efficiency in finding association patterns.

2. [Time Series Models](https://github.com/haroldeustaquio/Data-Mining-UNAM/blob/main/sales-beverage/time_series.ipynb):
   - **``ARIMA``**: Analyzes and predicts sales trends over time.
   - **``Triple Exponential Smoothing``**: Provides more accurate demand projections.

---

### [2. Sales Transaction](https://github.com/haroldeustaquio/Data-Mining-UNAM/tree/main/sales-transaction)

#### Overview
The Sales Transaction project focuses on analyzing product transaction data to identify customer purchasing patterns and trends. It applies clustering, classification, and regression models to derive actionable insights.

#### Models Applied
1. [Clustering Algorithms](https://github.com/haroldeustaquio/Data-Mining-UNAM/blob/main/sales-transaction/clustering.ipynb):  
   - **``K-Means Clustering``**: Partitions data points into clusters based on proximity.
   - **``Agglomerative Clustering``**: Merges similar data points to form a hierarchy of clusters.

2. [Classification Algorithms](https://github.com/haroldeustaquio/Data-Mining-UNAM/blob/main/sales-transaction/classification.ipynb):  
   - **``Decision Trees``**: Segments data through hierarchical splits for clear interpretations.
   - **``Logistic Regression``**: Models binary classifications through a sigmoid function.

3. [Regression Algorithms](https://github.com/haroldeustaquio/Data-Mining-UNAM/blob/main/sales-transaction/regression.ipynb):  
   - **``DecisionTreeRegressor``**: Predicts continuous values by recursively splitting data.
   - **``GradientBoostingRegressor``**: Improves prediction accuracy by combining weak models.

---

### [3. Neural Network](https://github.com/haroldeustaquio/Data-Mining-UNAM/tree/main/neural-network)

#### Overview
This project implements a sequence-to-sequence (seq2seq) model using PyTorch, aimed at generating text based on sequences derived from the Harry Potter series. The model leverages an Encoder-Decoder architecture alongside word embedding techniques.

#### Models Applied
- **``Encoder-Decoder Architecture``**: Processes input sequences and generates output sequences.
- **``Word Embedding Techniques``**: Captures semantic relationships between words used in the series.

---

#### Requirements
To run any of the projects in this repository, ensure you have the following Python libraries installed:

```bash
# For Sales Beverage and Sales Transaction
pip install pandas numpy matplotlib scikit-learn seaborn shap
```

```bash
# For Seq2Seq Model
pip install torch==2.3.1 torchvision==0.18.1 torchaudio==2.3.1 --index-url https://download.pytorch.org/whl/cu121
pip install torchtext==0.18
```