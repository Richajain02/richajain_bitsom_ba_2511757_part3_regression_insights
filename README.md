# Retail Sales Regression Analysis

## Business Problem Summary

The leadership team of a retail chain wants to understand which factors are associated with monthly sales performance across stores. The objective is to identify key sales drivers and support business decisions related to marketing investment, inventory management, and store operations.

---

## Dataset Description

The dataset contains monthly performance information for 320 retail stores. Variables include sales performance, marketing activity, customer traffic, inventory availability, customer ratings, regional information, and store type classifications.

Data preparation included handling missing values and creating dummy variables for categorical features used in regression analysis.

---

## Dependent and Independent Variables

### Dependent Variable

* monthly_sales

### Independent Variables Evaluated

Numerical Variables:

* marketing_spend
* footfall
* avg_discount_pct
* inventory_availability_pct
* customer_rating
* competitor_distance_km

Categorical Variables:

* region
* store_type

---

## Regression Approach

The analysis was completed in three stages:

### Simple Regression Models

Model 1:

* Dependent Variable: monthly_sales
* Independent Variable: marketing_spend

Model 2:

* Dependent Variable: monthly_sales
* Independent Variable: footfall

### Multiple Regression Model

Dependent Variable:

* monthly_sales

Independent Variables:

* marketing_spend
* footfall
* inventory_availability_pct
* region_North

The multiple regression model was selected as the final model because it provided the highest explanatory power.

---

## Dummy Variable Approach

Categorical variables were converted into dummy variables before regression analysis.

### Region

Created:

* region_North
* region_South
* region_West

Reference Category:

* East

### Store Type

Created:

* store_Airport
* store_High Street
* store_Mall

Reference Category:

* Residential

Reference categories were excluded to avoid the dummy variable trap and prevent multicollinearity.

---

## Model Comparison Summary

| Model               | Variables Used                                                    | R²     |
| ------------------- | ----------------------------------------------------------------- | ------ |
| Simple Regression 1 | Marketing Spend                                                   | 0.1672 |
| Simple Regression 2 | Footfall                                                          | 0.7363 |
| Multiple Regression | Marketing Spend, Footfall, Inventory Availability %, Region_North | 0.8046 |

The multiple regression model achieved the highest explanatory power and was selected as the preferred model.

---

## Final Model Selected

### Multiple Regression Model

Monthly Sales = 135,425.92 + 1.18(Marketing Spend) + 33.66(Footfall) + 2924.49(Inventory Availability %) − 1027.69(Region_North)

Model Performance:

* R² = 0.8046
* Adjusted R² = 0.8021

---

## Business Recommendation

The analysis indicates that the factors most strongly associated with monthly sales are:

1. Footfall
2. Inventory Availability Percentage
3. Marketing Spend

Recommendations:

* Increase customer footfall through promotions and customer engagement initiatives.
* Maintain high inventory availability to reduce stockouts and lost sales opportunities.
* Continue investing in marketing while monitoring return on investment.
* Investigate stores with unusually large residuals to identify operational strengths and weaknesses.

Regional differences should not be heavily emphasized because the Region_North variable was not statistically significant.

---

## Assumptions and Limitations

* Regression analysis identifies associations rather than causation.
* Some factors influencing sales may not be included in the dataset.
* Results are based on historical data and may not fully predict future conditions.
* Individual store performance may be affected by local factors not captured in the model.
* The model explains approximately 80.46% of sales variation, leaving some unexplained variability.

---

## Screenshots Included

The following supporting screenshots are included:

* screenshots/simple_regression_output.png
* screenshots/multiple_regression_output.png
* screenshots/model_comparison_preview.png
* screenshots/residuals_preview.png

These screenshots provide evidence of regression outputs, model comparison results, and residual analysis findings.

