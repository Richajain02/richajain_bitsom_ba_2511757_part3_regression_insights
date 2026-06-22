# Final Recommendation

## Executive Summary

Regression analysis was conducted to identify the factors most strongly associated with monthly sales performance across retail stores. Three models were evaluated: a simple regression using marketing spend, a simple regression using footfall, and a multiple regression model incorporating marketing spend, footfall, inventory availability, and region.

The multiple regression model was selected as the final model because it provided the highest explanatory power (R² = 0.8046), meaning it explained approximately 80.46% of the variation in monthly sales.

---

## Which Factors Are Most Strongly Associated with Monthly Sales?

The analysis indicates that the following factors are most strongly associated with monthly sales:

1. **Footfall**

   * Coefficient: 33.66
   * P-value: 2.26E-99
   * Strong positive relationship with sales.

2. **Inventory Availability Percentage**

   * Coefficient: 2924.49
   * P-value: 4.08E-09
   * Higher inventory availability is associated with higher sales.

3. **Marketing Spend**

   * Coefficient: 1.18
   * P-value: 8.55E-17
   * Increased marketing investment is associated with increased sales.

Among these variables, footfall appears to be the strongest predictor of sales performance.

---

## Which Variables Should Leadership Focus On?

Leadership should prioritize:

### Increasing Customer Footfall

The analysis shows that customer traffic has the strongest relationship with monthly sales. Strategies that attract more customers into stores are likely to have the greatest impact on revenue growth.

Possible actions include:

* Local marketing campaigns
* Promotional events
* Loyalty programs
* Improved store visibility and customer experience

### Maintaining High Inventory Availability

Inventory availability was found to be a significant driver of sales. Stock shortages may result in lost sales opportunities.

Possible actions include:

* Improving inventory planning
* Reducing stockouts
* Enhancing supply chain coordination
* Monitoring fast-moving products more closely

### Optimizing Marketing Spend

Marketing spend contributes positively to sales and should continue to be used strategically. However, marketing investments should be evaluated based on their ability to increase customer footfall and conversion rates.

---

## Which Variables Should Not Be Over-Interpreted?

### Region_North

The Region_North dummy variable had a coefficient of -1027.69 but a p-value of 0.874.

Because the p-value is substantially greater than 0.05, there is insufficient evidence to conclude that stores in the North region perform differently from stores in the reference region (East) after accounting for other factors.

Leadership should avoid making major strategic decisions based solely on regional differences identified in this model.

---

## Recommended Business Actions

Based on the regression results, the following actions are recommended:

1. Focus on initiatives that increase store footfall.
2. Maintain high inventory availability to minimize lost sales opportunities.
3. Continue investing in marketing while monitoring return on investment.
4. Investigate stores with unusually large positive or negative residuals to identify operational best practices or performance issues.
5. Use the multiple regression model as a forecasting and planning tool for future sales analysis.

---

## Risks and Limitations

Several limitations should be considered when interpreting the results:

* The model explains approximately 80.46% of sales variation, meaning other factors still influence performance.
* Variables not included in the dataset may affect sales outcomes.
* Market conditions may change over time.
* Individual stores may behave differently due to local factors that are not captured by the model.
* Regression models rely on historical data and may not fully predict future business conditions.

---

## Why Regression Does Not Prove Causation

Regression analysis identifies statistical associations between variables, but it does not automatically prove that one variable directly causes another.

For example, higher footfall is associated with higher sales, but this does not necessarily mean footfall alone causes increased sales. Other factors, such as promotions, store quality, product assortment, or local market conditions, may influence both footfall and sales simultaneously.

Similarly, higher marketing spend is associated with higher sales, but regression alone cannot prove that increasing marketing spend will always produce proportional sales growth.

Therefore, regression results should be used as decision-support evidence rather than proof of cause-and-effect relationships.

---

## Final Conclusion

The multiple regression model was selected as the final model because it provides the strongest explanation of monthly sales performance (R² = 0.8046).

The analysis indicates that footfall, inventory availability, and marketing spend are the most important factors associated with sales. Leadership should prioritize actions that increase customer traffic, maintain product availability, and optimize marketing investments while recognizing that regression identifies associations rather than definitive causal relationships.

