# hrishikeshpatil_bitsom_ba_2511159_part3_regression_insights

Part 3: Regression-Based Business Insights & Model Interpretation

Business Problem Summary

In this project, I analyzed a retail store dataset to understand which business factors are associated with monthly sales. The main objective was to identify whether variables such as marketing spend, customer footfall, inventory availability, discounts, customer ratings, and store characteristics have an impact on sales performance.

The results of this analysis can help the management team make better business decisions related to marketing, inventory planning, staffing, and overall store performance.


Dataset Description

The dataset contains monthly business information collected from different retail stores. Each row represents the performance of one store during a particular month.

The dataset includes information such as marketing spend, customer footfall, average discount offered, staff count, inventory availability, customer ratings, store type, region, monthly sales, and monthly profit.

For this analysis, monthly_sales is used as the target variable because the objective is to understand which factors influence sales.



Dependent Variable

monthly_sales

Monthly sales is the dependent variable because it is the value that the regression models are trying to predict.



Independent Variables

The following variables were selected as independent variables:

- marketing_spend
- footfall
- avg_discount_pct
- staff_count
- inventory_availability_pct
- competitor_distance_km
- holiday_flag
- customer_rating
- region
- store_type

These variables were chosen because they are likely to influence monthly sales.



Numerical Variables

The numerical variables available in the dataset are:

- marketing_spend
- footfall
- avg_discount_pct
- staff_count
- inventory_availability_pct
- competitor_distance_km
- customer_rating
- monthly_sales
- monthly_profit

These variables contain numeric values and can be used directly in regression analysis.



Categorical Variables

The dataset contains two categorical variables:

- region
- store_type

Since regression analysis cannot work directly with text values, these variables will be converted into dummy variables before building the multiple regression model.



Variables Not Used

Two variables were excluded from the regression analysis.

store_id was not used because it is only a unique identifier for each store and does not provide any useful information for predicting sales.

monthly_profit was also excluded because profit is another business outcome that is closely related to sales. Including it as an independent variable could lead to misleading results.



Data Preparation

Before starting the regression analysis, the dataset was checked to ensure that it was suitable for analysis.

The following steps were performed:

- Verified that numerical columns were stored as numbers.
- Checked categorical variables for consistent values.
- Reviewed the dataset for duplicate records.
- Checked for missing values.
- Kept the original dataset unchanged and prepared a separate cleaned version for analysis.

These steps helped improve the quality of the data before building the regression models.



Regression Approach

The regression analysis was carried out in three stages.

First, simple linear regression models were created to study the relationship between monthly sales and one independent variable at a time.

Next, a multiple linear regression model was developed using several numerical variables together.

Finally, dummy variables were added for the categorical variables so that they could also be included in the final regression model.

The dependent variable used in all models is monthly_sales.



Dummy Variable Approach

The variables region and store_type contain text values, so they were converted into dummy variables.

One category from each variable was kept as the reference category. This approach helps avoid multicollinearity and ensures that the regression model produces reliable coefficient estimates.



Business Objective

The purpose of this analysis is to answer a few important business questions, such as:

- Does increasing marketing spend improve monthly sales?
- Is customer footfall strongly related to sales performance?
- Does better inventory availability help increase sales?
- Do customer ratings influence monthly sales?
- Are certain store types or regions performing better than others?

The answers to these questions will help management make more informed business decisions.



Assumptions and Limitations

This analysis is based only on the variables available in the provided dataset.

Regression analysis helps identify relationships between variables, but it does not prove that one variable directly causes changes in another.

Other factors, such as economic conditions, customer preferences, local competition, or seasonal trends, may also affect monthly sales but are not included in this dataset.



Repository Contents

This repository includes the following files:

- Dataset
- Regression Workbook
- Model Comparison
- Residual Analysis
- Regression Summary
- Model Equations
- Final Recommendation
- Required Screenshots
- README Documentation



Conclusion

This project uses regression analysis to study the factors that are associated with monthly sales in retail stores. The findings provide useful insights into which business variables have the strongest relationship with sales performance. These insights can support management in making data-driven decisions while also considering the limitations of statistical analysis.
