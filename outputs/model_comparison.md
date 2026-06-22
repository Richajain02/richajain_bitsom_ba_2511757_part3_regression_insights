# Model Comparison

## Overview

Three regression models were developed to understand the factors associated with monthly sales performance across stores.

---

## Model 1: Marketing Spend

### Variables Used

Dependent Variable:

* Monthly Sales

Independent Variable:

* Marketing Spend

### Performance

* R² = 0.1672
* P-value = 2.48E-14

### Significant Variables

* Marketing Spend

### Business Usefulness

Marketing spend is positively associated with sales and is statistically significant. However, the model explains only 16.72% of the variation in sales.

### Limitations

The model ignores customer traffic, inventory availability, and other business factors that influence sales performance.

---

## Model 2: Footfall

### Variables Used

Dependent Variable:

* Monthly Sales

Independent Variable:

* Footfall

### Performance

* R² = 0.7363
* P-value = 4.75E-94

### Significant Variables

* Footfall

### Business Usefulness

Footfall is a very strong predictor of sales performance. The model explains 73.63% of the variation in monthly sales.

### Limitations

Although highly predictive, the model does not account for marketing activities, inventory levels, or store characteristics.

---

## Model 3: Multiple Regression

### Variables Used

Dependent Variable:

* Monthly Sales

Independent Variables:

* Marketing Spend
* Footfall
* Inventory Availability Percentage
* Region_North

### Performance

* R² = 0.8046

### Significant Variables

* Marketing Spend
* Footfall
* Inventory Availability Percentage

Region_North was not statistically significant.

### Business Usefulness

This model provides the strongest explanation of sales performance and captures the combined effects of multiple business drivers. It is the most useful model for decision-making.

### Limitations

The model identifies associations rather than causation. Other factors not included in the dataset may also affect sales performance.

---

## Final Assessment

Among the three models, the multiple regression model is the preferred model because it has the highest explanatory power (R² = 0.8046) and incorporates several important business drivers simultaneously.

Footfall appears to be the strongest individual predictor of sales, while inventory availability and marketing spend also contribute positively to store performance.
