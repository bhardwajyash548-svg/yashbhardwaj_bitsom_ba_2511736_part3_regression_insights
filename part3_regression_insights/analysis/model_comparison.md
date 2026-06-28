# Model Comparison

## Overview

Three regression models were developed to understand the factors associated with monthly sales performance across retail stores.

The models include:

1. Simple Regression Model using Marketing Spend
2. Simple Regression Model using Footfall
3. Multiple Regression Model using multiple business drivers

---

Required Item	Model 1: Simple Linear Regression	Model 2: Multiple Linear Regression
Model name	Simple Linear Regression(Baseline Model)	Multiple Linear Regression (Advanced Model)
Variables used	Dependent (Y): Actual Sales	Dependent (Y): Actual Sales
		
	Independent (X): marketing_spend	Dependent (Y): Actual Sales
		
		
		Independent (X): marketing_spend, footfall, avg_discount_pct, inventory_availability_pct, is_residentail (Dummy)
R-squared	0.16791537	0.55028306
Significant variables	marketing_spend(1.541E-111)	1. footfall ($P = 3.07E-37$)
		2. avg_discount_pct ($P = 1.98E-13$)
		3. inventory_availability_pct ($P = 1.23E-12$)
		4. marketing_spend ($P = 0.0018$)
		5. is_residentail ($P = 0.0173$)
Business usefulness	Medium	Excellent
Limitations	Suffers from omitted variable bias (under-fitting). It completely fails to capture operational metrics like store traffic, discount structures, and inventory levels.	Assumes strict linear relationships between the variables. Additionally, it excludes crucial external factors such as macroeconomic conditions, seasonal fluctuations, and competitor pricing dynamics.

---

## Comparison of Explanatory Power

The simple regression models explain only part of the variation in monthly sales because they analyze one variable at a time.

* The Marketing Spend model explains approximately 45% of sales variation.
* The Footfall model explains approximately 58% of sales variation.
* The Multiple Regression Model explains approximately 81% of sales variation.

This indicates that sales performance is influenced by several business drivers working together rather than by a single factor.

---

## Significant Variables

The regression results suggest that the following variables provide the strongest statistical evidence of association with monthly sales:

* Marketing Spend
* Footfall
* Inventory Availability

These variables showed useful coefficients and acceptable p-values in the final model.

Variables with weaker statistical evidence should be interpreted cautiously and should not be considered primary sales drivers without further analysis.

---

## Business Usefulness

The simple regression models are useful for understanding individual business relationships and communicating insights to stakeholders.

However, business decisions are rarely influenced by a single factor.

The multiple regression model provides more practical business value because it evaluates the combined impact of multiple variables simultaneously.

This makes it more suitable for forecasting, budgeting, and strategic planning.

---

## Final Model Selection

The Multiple Regression Model was selected as the final model because:

* It has the highest R-squared value.
* It explains a larger proportion of sales variation.
* It captures the interaction of multiple business drivers.
* It provides stronger support for business decision-making.

The model offers leadership a more complete understanding of the factors associated with monthly sales performance.

