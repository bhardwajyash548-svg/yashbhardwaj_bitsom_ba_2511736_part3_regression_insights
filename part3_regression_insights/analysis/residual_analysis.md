# Residual Analysis

## Overview

Residual analysis was performed using the selected multiple regression model to evaluate how accurately the model predicts monthly sales across stores.

Predicted sales values were calculated using the final regression equation, and residuals were calculated using the following formula:

Residual = Actual Monthly Sales − Predicted Monthly Sales

A positive residual means actual sales were higher than predicted sales.

A negative residual means actual sales were lower than predicted sales.

---

## Largest Positive Residuals

The following records showed the largest positive residual values:

 | Actual Sales | Predicted Sales | Residual |
 | ------------ | --------------- | -------- |
 | 810446.53    | 138676.5        | 61898.87795|
 | 758827.64    | 109432.6        | 52006.87166|
 | 828219.67    | 129761.7.       | 50045.16752|
 | 870937.4     | 126051.8        | 49230.98255|
 | 727241.86    | 106874.2        | 48936.06039|

### Business Interpretation

These stores performed significantly better than the model expected.

Possible explanations include:

* Highly effective local store management.
* Strong local customer loyalty.
* Temporary promotional campaigns.
* Favorable local market conditions.
* Competitor store closures nearby.

These factors may not be included in the regression model and therefore could not be captured in the predictions.

---

## Largest Negative Residuals

The following records showed the largest negative residual values:

| Record ID | Actual Sales | Predicted Sales | Residual |
| --------- | ------------ | --------------- | -------- |
| Store 7   | 914544.17    | 138573.6.       | -58741.83419|
| Store 18  | 685379.08    | 155311.4        | -48412.60751|
| Store 29  | 671868.59    | 117037.2.       | -46033.9394 |
| Store 41  | 680840.36    | 104966.1        | -36958.41941|
| Store 53  | 682639.28    | 112217.3        | -34659.81245|

### Business Interpretation

These stores generated lower sales than the model expected.

Possible explanations include:

* Inventory shortages.
* Local competition.
* Operational challenges.
* Staffing issues.
* Reduced customer demand in specific locations.

These factors were not directly included in the regression model.

---

## Under-Prediction and Over-Prediction Patterns

The model appears to under-predict certain high-performing stores that consistently outperform expectations.

These stores may benefit from:

* Strong local management teams.
* Better customer service quality.
* Unique local demand conditions.

The model also appears to over-predict certain lower-performing stores where operational or market challenges may exist.

This suggests that additional variables could improve future model performance.

Potential variables include:

* Competitor density
* Seasonal effects
* Local demographics
* Promotional campaign effectiveness
* Staff productivity measures

---

## Overall Assessment

The residual values indicate that the model performs reasonably well for most stores but does not fully explain all sales variation.

This is expected because retail sales are influenced by many factors beyond those included in the regression model.

Residual analysis provides valuable insights into where the model performs well and where additional business variables may improve prediction accuracy.

The results support the use of the multiple regression model as a decision-support tool while recognizing its limitations.

