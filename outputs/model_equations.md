Model Equations


Simple Regression Model 1

Dependent Variable: monthly_sales

Independent Variable: marketing_spend

Regression Equation

Monthly Sales = Intercept + (Coefficient × Marketing Spend)

Example:

Monthly Sales = __ + (__ × Marketing Spend)

Interpretation

In this model, I checked whether marketing spend has any relationship with monthly sales. The intercept represents the estimated sales when marketing spend is zero, while the coefficient shows how sales are expected to change when marketing spend increases by one unit.

If the coefficient is positive, it means stores that spend more on marketing generally tend to have higher sales.



Simple Regression Model 2

Dependent Variable: monthly_sales

Independent Variable: footfall

Regression Equation

Monthly Sales = Intercept + (Coefficient × Footfall)

Example:

Monthly Sales = __ + (__ × Footfall)

Interpretation

This model helps understand how customer footfall is related to monthly sales. The coefficient tells us how much the sales are expected to change when the number of customer visits increases.

A positive coefficient indicates that stores with higher customer footfall usually achieve better sales.



Multiple Regression Model

For the final model, I included several business variables together instead of analysing only one factor at a time.

Variables Used

- marketing_spend
- footfall
- avg_discount_pct
- staff_count
- inventory_availability_pct
- Region Dummy Variables
- Store Type Dummy Variables

Final Regression Equation

Monthly Sales =

114687.202

+ (1.164070198 × Marketing Spend)

+ (28.70319921 × Footfall)

− (47096.9846 × Average Discount %)

+ (2853.233001 × Staff Count)

+ (2956.046845 × Inventory Availability %)

+ (7700.568958 × Region_North)

+ (19440.62508 × Region_South)

+ (18502.25223 × Region_West)

+ (21712.02719 × Store_Airport)

+ (11909.7725 × Store_Mall)

− (17398.20911 × Store_Residential)



Understanding the Results

The coefficient of marketing_spend is positive, which suggests that stores spending more on marketing generally have higher monthly sales.

The positive coefficient for footfall indicates that stores receiving more customer visits are likely to generate higher sales.

The average discount percentage has a negative coefficient. This suggests that offering higher discounts may reduce overall monthly sales value, although discounts can still help increase customer purchases in some situations.

Both staff_count and inventory_availability_pct have positive coefficients. This indicates that having enough staff and maintaining product availability may contribute to better sales performance.

The dummy variables for region and store type show that store location and store format also have some influence on monthly sales when compared with their reference categories.



Dummy Variables

Since region and store_type are categorical variables, I converted them into dummy variables before running the regression analysis.

For the region variable, I selected East as the reference category and created dummy variables for North, South, and West.

For store_type, one category was kept as the reference category, while dummy variables were created for the remaining store types.

Using a reference category helps avoid duplicate information in the regression model and makes the results easier to interpret.



Final Model Selection

After comparing all the models, I selected the multiple regression model as the final model for this project.

I felt this model was the best choice because monthly sales are influenced by many factors working together, not just one. By considering marketing spend, customer footfall, discounts, staff count, inventory availability and store characteristics in the same model, the results provide a much better understanding of sales performance.

The final model also achieved an R-squared value of 0.8305, which means it explains around 83% of the variation in monthly sales. Based on these results, I believe this model is the most suitable for supporting business decisions in this project.