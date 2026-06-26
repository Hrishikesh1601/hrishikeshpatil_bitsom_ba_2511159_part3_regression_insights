hrishikeshpatil_2511159_part3_regression_insights

Part 3: Regression-Based Business Insights & Model Interpretation

Business Problem Summary

In this project, I analyzed a retail store dataset to understand which business factors are associated with monthly sales. The aim was to identify how variables like marketing spend, customer footfall, discounts, staff count, inventory availability, region, and store type are related to sales performance.

The findings from this analysis can help management make better decisions regarding marketing, inventory planning, staffing, and overall store operations.



Dataset Description

The dataset contains monthly business information for different retail stores. Each record represents the performance of one store for a particular month.

The dataset includes details such as marketing spend, customer footfall, average discount percentage, staff count, inventory availability, region, store type, monthly sales and monthly profit.

For this project, monthly_sales was selected as the dependent variable because the main objective was to understand the factors associated with sales performance.



Dependent Variable

monthly_sales

Monthly sales is the target variable that all regression models are trying to predict.



Independent Variables

The following variables were used in the final regression model:

- marketing_spend
- footfall
- avg_discount_pct
- staff_count
- inventory_availability_pct
- region (converted into dummy variables)
- store_type (converted into dummy variables)



Numerical Variables

The dataset contains several numerical variables, including:

- marketing_spend
- footfall
- avg_discount_pct
- staff_count
- inventory_availability_pct
- competitor_distance_km
- customer_rating
- monthly_sales
- monthly_profit

Only the variables required for the final regression model were used in the analysis.



Categorical Variables

The dataset contains two categorical variables:

- region
- store_type

Since regression analysis requires numerical inputs, these variables were converted into dummy variables before building the multiple regression model.



Variables Not Used

Some variables were not included in the final regression model.

- store_id was excluded because it is only a unique identifier.
- monthly_profit was excluded because it is another business outcome and could lead to data leakage.
- customer_rating was excluded because it contained missing values.
- competitor_distance_km and holiday_flag were not included in the final model selected for this analysis.



Data Preparation

Before performing the regression analysis, I prepared the dataset by following these steps:

- Verified that numerical columns contained numeric values.
- Checked categorical variables for consistency.
- Reviewed the dataset for duplicate records.
- Checked for missing values.
- Kept the original dataset unchanged.
- Created a separate cleaned dataset for regression analysis.
- Converted categorical variables into dummy variables.



Regression Approach

The analysis was completed in three stages.

First, I created simple regression models to understand the relationship between monthly sales and one independent variable at a time.

Next, I built a multiple regression model using several numerical variables together.

Finally, I added dummy variables for region and store_type to include categorical information in the final model.


Dummy Variable Approach

The variables region and store_type were converted into dummy variables before running the regression analysis.

For the region variable, East was used as the reference category, while dummy variables were created for North, South, and West.

Similarly, one category from store_type was used as the reference category, and dummy variables were created for the remaining store types.

Using a reference category helps avoid multicollinearity and makes the regression results easier to interpret.



Business Objective

The purpose of this analysis was to answer questions such as:

- Does higher marketing spend relate to higher monthly sales?
- Does customer footfall have an impact on sales?
- Does inventory availability improve sales performance?
- How do discounts affect monthly sales?
- Do different regions and store types perform differently?

The answers to these questions can help management make better business decisions based on data.



Assumptions and Limitations

This analysis is based only on the variables available in the provided dataset.

Regression analysis helps identify relationships between variables, but it does not prove that one variable directly causes another.

Other factors such as customer behaviour, seasonal demand, weather, local competition, festivals and economic conditions may also affect monthly sales but were not included in this dataset.



Repository Contents

This repository contains:

- Dataset
- Regression Workbook
- Model Comparison
- Residual Analysis
- Regression Summary
- Model Equations
- Final Business Recommendation
- Required Screenshots
- README Documentation



Conclusion

This project helped me understand how regression analysis can be used to identify the business factors associated with monthly sales. After comparing different models, I selected the multiple regression model because it explained the data better and provided more meaningful business insights.

Although no regression model can perfectly predict future sales, the results of this analysis can support management in making better business decisions based on available data.
