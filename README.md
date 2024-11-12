# Data-Mining-UNAM

## Overview
This repository contains several projects from the Data Mining course at UNAM, Mexico. These projects were developed throughout the semester 24-2, with each one being presented and detailed extensively. The aim of these projects is to extract valuable insights from various datasets relevant to customer behavior, sales transactions, and text generation based on the Harry Potter series.


**Content:**
* [Sales Beverage](#sales-beverage)
* [Sales Transaction](#sales-transaction)
* [Neural Network](#neural-network)
* [Final Project](#final-project)
* [Requirements](#requirements)

---

## Sales Beverage

The Sales Beverage project analyzes transaction data for isotonic drinks, utilizing association and time series models to identify purchasing patterns and trends in customer behavior. The ultimate goal is to enhance marketing and sales strategies for beverage companies.

* [Association Models](https://github.com/haroldeustaquio/Data-Mining-UNAM/blob/main/sales-beverage/association.ipynb) :
   - **``Apriori``**: Finds frequent relationships between purchased products.
   - **``FP-Growth``**: Improves efficiency in finding association patterns.

* [Time Series Models](https://github.com/haroldeustaquio/Data-Mining-UNAM/blob/main/sales-beverage/time_series.ipynb):
   - **``ARIMA``**: Analyzes and predicts sales trends over time.
   - **``Triple Exponential Smoothing``**: Provides more accurate demand projections.

---

## Sales Transaction

The Sales Transaction project focuses on analyzing product transaction data to identify customer purchasing patterns and trends. It applies clustering, classification, and regression models to derive actionable insights.

* [Clustering Algorithms](https://github.com/haroldeustaquio/Data-Mining-UNAM/blob/main/sales-transaction/clustering.ipynb):  
   - **``K-Means Clustering``**: Partitions data points into clusters based on proximity.
   - **``Agglomerative Clustering``**: Merges similar data points to form a hierarchy of clusters.

* [Classification Algorithms](https://github.com/haroldeustaquio/Data-Mining-UNAM/blob/main/sales-transaction/classification.ipynb):  
   - **``Decision Trees``**: Segments data through hierarchical splits for clear interpretations.
   - **``Logistic Regression``**: Models binary classifications through a sigmoid function.

* [Regression Algorithms](https://github.com/haroldeustaquio/Data-Mining-UNAM/blob/main/sales-transaction/regression.ipynb):  
   - **``DecisionTreeRegressor``**: Predicts continuous values by recursively splitting data.
   - **``GradientBoostingRegressor``**: Improves prediction accuracy by combining weak models.

---

## Neural Network

This project implements a sequence-to-sequence (seq2seq) model using PyTorch, aimed at generating text based on sequences derived from the Harry Potter series. The model leverages an Encoder-Decoder architecture alongside word embedding techniques.

- **``Encoder-Decoder Architecture``**: Processes input sequences and generates output sequences.
- **``Word Embedding Techniques``**: Captures semantic relationships between words used in the series.

---

## Final Project

This project aims to analyze the trends and patterns in oncological care during 2022 to identify gaps in coverage and improve service quality for cancer patients in Peru. By examining patient data across departments and demographic factors, the analysis provides insights for optimizing resources and enhancing accessibility in high-demand areas.

- **``Time Series Analysis (ARIMA)``**: Used to analyze and forecast the monthly number of oncological care visits.
- **``Classification Models``** (``RandomForestClassifier``, ``Logistic Regression``, ``ComplementNB``, ``CategoricalNB``, ``DecisionTreeClassifier``): Applied to predict the type of service required (e.g., consultation, teleorientation) based on patient characteristics.
- **``Clustering Models``** (``KMeans``, ``DBSCAN``): Used for patient segmentation to identify similar groups based on demographic and diagnostic characteristics.

---

## Requirements
To run any of the projects in this repository, ensure you have the following Python libraries installed:

```bash
# 'Sales Transaction', 'Sales Beverage' and 'Final Project'
pip install pandas numpy matplotlib scikit-learn seaborn statsmodels mlxtend shap

```

```bash
# For Seq2Seq Model
pip install torch==2.3.1 torchvision==0.18.1 torchaudio==2.3.1 --index-url https://download.pytorch.org/whl/cu121
pip install torchtext==0.18
```
----

