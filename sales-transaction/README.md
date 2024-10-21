# Sales Transaction

## Project overview

This project focuses on analyzing transaction data for products, with the goal of identifying purchasing patterns and trends in customer behavior. Utilizing Machine Learning techniques, **``clustering techniques``**, **``classification models``**, moreover, **``regression models``** were implemented to extract valuable insights that can help companies optimize their marketing and sales strategies.

---

## Business context

The dataset comes from a company that seeks to optimize its marketing and sales strategies based on customer behavior. The main objectives of this analysis are:

- **Segment customers**: Group customers into segments based on demographic characteristics (such as age, marital status, education level) and purchasing patterns (such as product preferences, spending habits).
- **Product sector analysis**: Analyze product sectors to identify sales trends and customer behavior for specific categories, lines, and sublines.

By leveraging clustering, the company aims to:

- **Personalize marketing strategies**: Tailor marketing campaigns to each customer segment, offering relevant products and promotions.
- **Identify new business opportunities**: Discover potential markets or customer needs that can be addressed with new product development or expansion into different sectors.
- **Improve customer experience**: Provide more personalized services, improving customer satisfaction and loyalty by understanding their specific needs and preferences.

---

## Data Description

The dataset contains a wide variety of variables relevant to customer purchasing and demographics:

- **Product-related variables**: `Industry`, `Type`, `Line`, `Subline`, `Presentation`, `Weight`, `Product`, `Description`
- **Transaction details**: `Date`, `Transaction`, `Order`, `Quantity`, `Price`, `Max_Price`, `Max_Price_Dif`, `Amount`
- **Customer demographics**: `Customer`, `Customer_Key`, `No._Children`, `Seniority`, `Age`, `Age_Range`, `Education`, `Marital_Status`, `State`, `Sex`
- **Business identifiers**: `Company`, `Year`
- **Other variables**: `Function`, `Group`

These variables provide detailed information about the purchasing behavior of customers, allowing the company to better understand both their demographic characteristics and how they interact with different product categories.

---
## Models Applied
Three types of Machine Learning models were used in this analysis:

1. **Clustering Algorithms**:  
   - **K-Means Clustering**: This algorithm partitions data points into clusters based on proximity to cluster centers.  
   - **Agglomerative Clustering**: This method builds a hierarchy of clusters by merging similar data points, starting with each point as an individual cluster.

2. **Classification Algorithms**:  
   - **Decision Trees**: A model that segments data through hierarchical splits, offering clear visual interpretations of decision-making.  
   - **Logistic Regression**: This statistical model predicts class probabilities, effectively modeling binary classifications through a sigmoid function.

3. **Regression Algorithms**:  
   - **DecisionTreeRegressor**: This model predicts continuous values by recursively splitting data, capturing complex relationships while remaining interpretable.  
   - **GradientBoostingRegressor**: An ensemble method that sequentially improves prediction accuracy by combining weak models, effectively managing non-linear relationships.
   
--- 

## Requirements

Make sure you have the following Python libraries installed:

- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`
- `seaborn`
- `shap`