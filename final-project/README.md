# Final Project
## Oncological Coverage 2022: An Analysis of Impact and Trends in Peru

## Overview
This project aims to analyze the trends and patterns in oncological care during 2022 to identify gaps in coverage and improve service quality for cancer patients in Peru. By examining patient data across departments and demographic factors, the analysis provides insights for optimizing resources and enhancing accessibility in high-demand areas. The goal is to enable FISSAL and IPRESS to identify regions with high oncological care demand, optimize resource allocation, and ultimately improve the quality of life for cancer patients.

* Open Data: https://www.datosabiertos.gob.pe/dataset/atenciones-de-cobertura-oncol%C3%B3gica-periodos-2022-2023-fondo-intangible-solidario-de-salud
* Report: https://bit.ly/45SZeu7


**Content**
* [Problem Statement](#problem-statement)
* [Benefits](#benefits)
* [CRISP-DM Methodology](#crisp-dm-methodology)
* [Situations and Models Applied](#situations-and-models-applied)
* [Requirements](#requirements)

---

## Problem Statement
   - **Unequal Distribution of Services**: Certain regions experience limited access to oncological care.
   - **Resource Optimization**: There's a need to allocate resources more efficiently based on demand.
   - **Personalized Care Approach**: Differentiating care strategies according to patient profiles (age, gender, cancer type).

---

## Benefits
   - **Improved Accessibility**: Expanding access to essential cancer care services, especially in underserved regions.
   - **Efficient Resource Allocation**: Optimizing the use of medical resources based on demand patterns helps reduce wastage and improve service availability.
   - **Patient-Centered Care Approach**: Tailoring services based on patient demographics and needs, such as age and type of cancer, can enhance treatment outcomes.

---

## CRISP-DM Methodology

**Business Understanding**  
   - **Objective**: Identify how oncological data analysis can improve coverage and resource distribution in Peru.
   - **Key Questions**: 
      - What are the most common types of cancer treated?
      - Which regions have the highest demand?
      - What is the patient profile in terms of age, gender, and insurance type?

**Data Understanding**  
   - **Objective**: Collect and understand data on consultations, diagnoses, demographics, and insurance types.
   - **Initial Exploration**: Examine consultation distributions by department, cancer type, and patient demographics.

**Data Preparation**  
   - **Objective**: Clean and preprocess data to ensure quality and relevance for modeling.
   - **Activities**:
      - Data Cleaning
      - Variable Transformation
      - Selection of Key Variables

**Modeling**  
   - **Objective**: Apply suitable algorithms for analysis and prediction.
   - **Models Used**:
      - **Time Series Analysis** (e.g., ARIMA) for predicting monthly patient numbers.
      - **Logistic Regression, Naive Bayes, Clustering** for different aspects of patient and service prediction.

**Evaluation**  
   - **Objective**: Validate model accuracy and practicality.
   - **Model Selection**: Choose models based on performance metrics to ensure they meet business objectives.

**Deployment**  
   - **Objective**: Implement the model and create interactive visualizations.
   - **Activities**:
      - Dashboard Creation
      - Report Generation

---

## Situations and Models Applied

### Situation 1: Service Type Classification
   - **Objective**: Predict the type of service needed based on patient characteristics.
   - **Models**: ``RandomForestClassifier``, ``Logistic Regression``, ``ComplementNB``, ``CategoricalNB``, ``DecisionTreeClassifier``.
   - **Conclusion**: CategoricalNB provides the best balance between precision and recall, making it reliable for balanced classifications.

### Situation 2: Patient Segmentation Analysis
   - **Objective**: Group patients into similar segments based on characteristics.
   - **Models**: ``Kmeans`` (Elbow Method), ``DBSCAN``.
   - **Conclusion**: Clusters highlight two main profiles:
      - Women of varying ages with breast cancer.
      - Young individuals with leukemia, mostly beneficiaries of SIS Gratuito in Lima.

### Situation 3: Monthly Patient Count Time Series Model
   - **Objective**: Analyze trends in monthly patient counts for common cancer diagnoses.
   - **Model**: ``ARIMA``
   - **Conclusion**: The trend shows an increase in oncological care until October 2022, followed by a drop at year-end. Projections for 2023 suggest a demand recovery, indicating a need for additional resources during high-demand months.

---

## Requirements

To run this project, install the required libraries using:

```bash
pip install pandas matplotlib scikit-learn statsmodels 
```