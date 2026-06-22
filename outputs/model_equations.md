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

