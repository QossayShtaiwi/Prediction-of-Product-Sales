# Prediction-of-Product-Sales
### A regression analysis and predictive model for retail sales forecasting
**Author:**: Qossay Shtaiwi
## Business Problem

The stakeholder needs to better anticipate sales at the product-and-outlet level in order to improve inventory planning, reduce stockouts and overstock, and support smarter marketing decisions. This project analyzes historical sales data to identify the key drivers of sales performance and builds a predictive model that estimates expected sales for a given product at a given outlet.

## Data

The dataset includes historical sales records across multiple retail outlets, with features describing both the product (e.g., weight, fat content, visibility, type, price) and the outlet (e.g., size, location type, establishment year). The dataset contains [X] observations and [Y] features.

## Methods

- Exploration of the data and identifying the features (8523 entries, 12 columns)
- Dropping duplicated values
- Standardized inconsistent category labels (e.g., merging duplicate fat 
  content labels).
- Identifying the target feature. 
- Split data into training and test sets to evaluate how well the model 
  generalizes to unseen data.
  
### Preprocessing 
- Cleaned missing values in key fields using imputation with median for numerical feature and moset frequent in catigorical ones.
- Encoded categorical features for use in modeling.
- Fit and Transform
- Tested multiple regression approaches with varying levels of model 
  complexity and regularization, selecting the final model based on test 
  set performance and generalization stability (not just training fit).

  ## Results

### Insight 1
<img width="558" height="393" alt="image" src="https://github.com/user-attachments/assets/4bc3dbb9-dab3-42bd-b56a-e76b2cc35004" />

This chart showes the relationship between the retail price for the products compared with their sales,  There a positive correlation, higher price, HIGHER sales

### Insight 2
<img width="589" height="390" alt="image" src="https://github.com/user-attachments/assets/6c0cdd6a-ae23-4913-953a-5537b6c7d3a2" />


this figure copare the oultlet type with with sales. Its obvious that Supermarket type 3 has the highest sales among all types of oulets

## Model

The final model selected explains roughly **60% of the variation in outlet sales** (R² = 0.595 on unseen test data), and its typical prediction is within about **$734** of actual sales figures (Mean Absolute Error). 

## Limitations & Next Steps

- The model explains about 60% of sales variation, meaning other   unmeasured factors (e.g., local competition, promotions, seasonality) still play a meaningful role and aren't captured here.
- Next steps could include incorporating additional external data sources and testing additional model types to further close the gap.

## For Further Information

For additional questions, please contact qusay.shtewi@gmail.com or view the full technical analysis.
