# Residual Analysis

## Overview

Residual analysis was performed using the final multiple regression model.

### Final Regression Equation

Predicted Sales = 135425.9204 + (1.17669452 × Marketing Spend) + (33.66128796 × Footfall) + (2924.489431 × Inventory Availability %) − (1027.687346 × Region_North)

### Residual Calculation

Residual = Actual Sales − Predicted Sales

A positive residual indicates that actual sales were higher than predicted by the model.

A negative residual indicates that actual sales were lower than predicted by the model.

---

## Largest Positive Residuals

The following stores had the largest positive residuals:

| Store ID | Actual Sales | Predicted Sales |  Residual |
| -------- | -----------: | --------------: | --------: |
| STR-1028 |    713611.16 |       602447.48 | 111163.68 |
| STR-1026 |    625514.04 |       523997.72 | 101516.32 |
| STR-1051 |    787715.51 |       687766.48 |  99949.03 |
| STR-1032 |    914544.17 |       815431.39 |  99112.78 |
| STR-1064 |    799046.94 |       702766.24 |  96280.70 |

### Interpretation

These stores generated substantially higher sales than predicted by the model. This suggests that factors not included in the regression model may be contributing to their performance.

Possible explanations include:

* Strong local management
* Higher customer loyalty
* Favorable store locations
* Local promotions or events
* Other operational advantages

The model is under-predicting performance for these stores.

---

## Largest Negative Residuals

The following stores had the largest negative residuals:

| Store ID | Actual Sales | Predicted Sales |   Residual |
| -------- | -----------: | --------------: | ---------: |
| STR-1017 |    685379.08 |       842407.38 | -157028.30 |
| STR-1012 |    595467.60 |       729943.73 | -134476.13 |
| STR-1009 |    641865.03 |       759645.45 | -117780.42 |
| STR-1001 |    658920.30 |       773926.54 | -115006.24 |
| STR-1023 |    627171.90 |       738177.14 | -111005.24 |

### Interpretation

These stores generated lower sales than predicted by the model.

Possible explanations include:

* Operational inefficiencies
* Strong competition
* Lower customer conversion rates
* Staffing challenges
* Temporary business disruptions

The model is over-predicting performance for these stores.

---

## Business Discussion

The residual analysis shows that while the regression model explains approximately 80.46% of the variation in monthly sales, some stores still perform substantially better or worse than expected.

The largest positive residuals indicate stores where additional business advantages may exist that are not captured by the model.

The largest negative residuals indicate stores where challenges may be reducing sales despite favorable predictor values.

No clear pattern suggests that the model consistently under-predicts or over-predicts a specific region or store type. However, individual stores exhibit performance differences that may require further investigation.

Overall, the residual analysis suggests that the model provides strong predictive performance but does not capture every factor influencing sales outcomes.

