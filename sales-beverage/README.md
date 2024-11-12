# Sales Beverage

## Overview
This project focuses on analyzing transaction data for beverage products, specifically isotonic drinks, with the goal of identifying purchasing patterns and trends in customer behavior. Utilizing Machine Learning techniques, **``association``** and **``time series models``** were implemented to extract valuable insights that can help companies optimize their marketing and sales strategies.

**Content:**
* [Business Context](#business-context)
* [Data Description](#data-description)
* [Models Applied](#models-applied)
* [Requirements](#requirements)


---

## Business Context

The dataset originates from a beverage company that aims to enhance its marketing and sales strategies by leveraging insights derived from customer behavior. The main objectives of this analysis are:

- **Segment customers**: Classify customers into distinct segments based on demographic characteristics (such as age, marital status, education level) and purchasing patterns (including preferences for specific beverage types and spending habits).
- **Product sector analysis**: Examine the isotonic drinks sector to identify sales trends and customer behavior related to various product categories, lines, and sublines.

By utilizing clustering techniques and other Machine Learning models, the company seeks to:

- **Personalize marketing strategies**: Customize marketing campaigns for each customer segment, presenting relevant products and promotions that align with their preferences.
- **Identify new business opportunities**: Uncover potential markets or unmet customer needs that can be addressed through new product development or diversification into different beverage categories.
- **Improve customer experience**: Deliver tailored services to enhance customer satisfaction and loyalty by gaining a deeper understanding of their specific preferences and requirements.

By implementing these strategies, the company aims to strengthen its position in the competitive beverage market, ultimately driving growth and profitability.

---

## Data Description

The dataset contains a wide variety of variables relevant to customer purchasing and demographics:

- **Product-related variables**: `Sector`, `Type`, `Line`, `Subline`, `Presentation`, `Weight`, `Product`, `Description`
- **Transaction details**: `Date`, `Transaction`, `Order`, `Quantity`, `Price`, `Max_Price`, `Price_Difference_Max`, `Amount`
- **Customer demographics**: `Client`, `Client_Key`, `Number_of_Children`, `Seniority`, `Age`, `Age_Range`, `Education`, `Marital_Status`, `State`, `Sex`
- **Business identifiers**: `Company`, `Year`
- **Other variables**: `Function`, `Group`


---
## Models Applied
Two types of Machine Learning models were used in this analysis:

1. **Association Models**:
   - **``Apriori``**: This algorithm was used to find frequent relationships between purchased products, allowing the identification of buying patterns and product recommendations.
   - **``FP-Growth``**: This method was implemented to improve efficiency in finding association patterns, successfully identifying combinations of products that customers tend to buy together.

2. **Time Series Models**:
   - **``ARIMA``**: This model was used to analyze and predict sales trends over time, helping to understand the seasonal and cyclical behavior of sales.
   - **``Triple Exponential Smoothing``**: This method was applied to smooth the time series and obtain more accurate projections of the demand for isotonic products.

---

## Requirements

To run this project, install the required libraries using:

```bash
pip install pandas numpy matplotlib scikit-learn seaborn statsmodels mlxtend
```