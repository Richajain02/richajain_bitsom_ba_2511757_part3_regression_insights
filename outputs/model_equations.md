# Dummy Variable Creation

## Purpose

Regression analysis requires numerical inputs. Since region and store_type are categorical variables, dummy variables were created to convert categories into numerical values that can be used in regression models.

---

## Region Dummy Variables

The region variable contains four categories:

* East
* North
* South
* West

East was selected as the reference category.

The following dummy variables were created:

* region_North
* region_South
* region_West

Example:

| Region | region_North | region_South | region_West |
| ------ | ------------ | ------------ | ----------- |
| East   | 0            | 0            | 0           |
| North  | 1            | 0            | 0           |
| South  | 0            | 1            | 0           |
| West   | 0            | 0            | 1           |

When all region dummy variables are equal to 0, the observation belongs to the East region.

---

## Store Type Dummy Variables

The store_type variable contains four categories:

* Residential
* Airport
* High Street
* Mall

Residential was selected as the reference category.

The following dummy variables were created:

* store_Airport
* store_High Street
* store_Mall

Example:

| Store Type  | store_Airport | store_High Street | store_Mall |
| ----------- | ------------- | ----------------- | ---------- |
| Residential | 0             | 0                 | 0          |
| Airport     | 1             | 0                 | 0          |
| High Street | 0             | 1                 | 0          |
| Mall        | 0             | 0                 | 1          |

When all store type dummy variables are equal to 0, the observation belongs to the Residential store category.

---

## Avoiding Dummy Variable Trap

One category from each categorical variable was used as the reference category. This prevents perfect multicollinearity and ensures the regression model can estimate coefficients correctly.

Reference Categories Used:

* Region: East
* Store Type: Residential

# Model Equations

## Overview

Regression analysis was conducted to identify factors associated with monthly sales performance across stores. Both simple regression and multiple regression models were developed and evaluated.

---

# Simple Regression Model 1

## Monthly Sales vs Marketing Spend

### Equation

Monthly Sales = 560,777.35 + 2.13 × Marketing Spend

### Coefficient Explanation

#### Intercept (560,777.35)

This represents the baseline monthly sales when marketing spend is zero.

#### Marketing Spend Coefficient (2.13)

For every additional unit spent on marketing, monthly sales are expected to increase by approximately 2.13 units on average.

### Business Meaning

The positive coefficient suggests that marketing investment contributes to sales growth. However, marketing spend alone explains only a limited portion of sales variation.

---

# Simple Regression Model 2

## Monthly Sales vs Footfall

### Equation

Monthly Sales = 446,410.58 + 35.68 × Footfall

### Coefficient Explanation

#### Intercept (446,410.58)

This represents the estimated sales level when customer footfall is zero.

#### Footfall Coefficient (35.68)

Each additional customer visit is associated with an increase of approximately 35.68 units in monthly sales.

### Business Meaning

Higher customer traffic is strongly associated with increased sales performance. Footfall appears to be one of the strongest individual drivers of sales.

---

# Multiple Regression Model

## Equation

Monthly Sales = 135,425.92 + 1.18(Marketing Spend) + 33.66(Footfall) + 2924.49(Inventory Availability %) − 1027.69(Region_North)

---

## Coefficient Explanations

### Intercept (135,425.92)

Represents the estimated monthly sales when all predictor variables are equal to zero.

### Marketing Spend (1.18)

Holding other variables constant, every additional unit increase in marketing spend is associated with an average increase of approximately 1.18 units in monthly sales.

### Footfall (33.66)

Holding other variables constant, each additional customer visit is associated with an increase of approximately 33.66 units in monthly sales.

### Inventory Availability Percentage (2924.49)

Stores with higher inventory availability tend to generate higher sales. This suggests that maintaining stock availability is important for maximizing revenue.

### Region_North (-1027.69)

After controlling for other variables, stores in the North region are estimated to have slightly lower sales than stores in the reference region. However, this effect was not statistically significant.

---

### Dummy Variables
Region was converted into dummy variables: region_North, region_South, and region_West.  
Store type was converted into dummy variables: store_Airport, store_High Street, and store_Mall.  
To avoid the dummy variable trap, one category from each variable was used as the reference category.  
Reference Categories -   
Variable	Reference Category  
Region	East  
Store Type	Residential  

The reference categories are represented when all dummy variables for that category are equal to 0.  

# Final Model Selected

Multiple Regression Model

Monthly Sales = 135,425.92 + 1.18(Marketing Spend) + 33.66(Footfall) + 2924.49(Inventory Availability %) − 1027.69(Region_North)

---

# Reason for Selecting the Final Model

The multiple regression model was selected because it provided the highest explanatory power among all models.

| Model               | R²     |
| ------------------- | ------ |
| Marketing Spend     | 0.1672 |
| Footfall            | 0.7363 |
| Multiple Regression | 0.8046 |

The multiple regression model explains approximately 80.46% of the variation in monthly sales, compared with 16.72% for the marketing spend model and 73.63% for the footfall model.

From a business perspective, the model captures several important drivers of sales simultaneously, including customer traffic, marketing investment, and inventory availability. This makes it more useful for decision-making and forecasting than relying on a single factor alone.

The results indicate that footfall, inventory availability, and marketing spend are the most important variables associated with monthly sales performance.


