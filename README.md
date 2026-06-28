# yashbhardwaj_bitsom_ba_2511736_part3_regression_insights

# Regression-Based Business Insights and Model Interpretation

## Business Problem Summary

The leadership team of a retail chain wants to understand which business factors are most strongly associated with monthly sales performance across stores.

The objective of this project is to use regression analysis to identify important sales drivers and provide business recommendations that can support decision-making related to marketing investment, inventory planning, discount strategy, staffing, and store operations.

---

## Dataset Description

The dataset contains store-level monthly business information including sales performance and operational variables.

The dataset includes variables such as:

* Monthly Sales
* Marketing Spend
* Footfall
* Average Discount Percentage
* Inventory Availability Percentage
* Customer Rating
* Store Type
* Region

The dataset was reviewed for missing values, duplicate records, invalid values, and inconsistencies before analysis.

---

## Dependent Variable

The dependent variable used in this analysis is:

**Monthly Sales**

Monthly sales were selected because the primary business objective is to understand the drivers of store revenue performance.

---

## Independent Variables

The following variables were considered as potential predictors of monthly sales:

* Marketing Spend
* Footfall
* Inventory Availability Percentage
* Average Discount Percentage
* Customer Rating
* Store Type Dummy Variables
* Region Dummy Variables

---

## Data Cleaning Approach

The dataset was cleaned before performing regression analysis.

The following checks were performed:

* Missing value identification
* Duplicate record detection
* Data type validation
* Numeric field verification
* Outlier review

The original dataset was preserved and all cleaning activities were performed on a separate cleaned dataset sheet.

---

## Regression Approach

Two types of regression models were developed:

### Simple Regression Models

Simple regression models were used to understand the relationship between monthly sales and individual business variables.

Examples include:

* Monthly Sales vs Marketing Spend
* Monthly Sales vs Footfall

### Multiple Regression Model

A multiple regression model was developed using multiple predictors simultaneously to provide a more realistic representation of business performance.

The final model included:

* Marketing Spend
* Footfall
* Inventory Availability Percentage
* Dummy Variables for Store Type

---

## Dummy Variable Approach

Categorical variables cannot be directly used in regression analysis.

Therefore, dummy variables were created for store type and selected categories were included in the regression model.

One category was excluded and used as the reference category to avoid multicollinearity and the dummy variable trap.

Reference Category:

**Hypermarket**

All dummy variable coefficients were interpreted relative to this category.

---

## Model Comparison Summary

Three regression models were evaluated:

| Model                     | Variables Used                                                               | R-Squared |
| ------------------------- | ---------------------------------------------------------------------------- | --------- |
| Simple Regression Model 1 | Marketing Spend                                                              | 0.16791537|
| Simple Regression Model 2 | Footfall                                                                     | 0.73830172|
| Multiple Regression Model | Marketing Spend, Footfall, Inventory Availability, Store Type Dummy Variable | 0.55028306|

The multiple regression model achieved the highest explanatory power and provided the most useful business insights.

---

## Final Model Selected

The Multiple Regression Model was selected as the final model because:

* It explained a larger proportion of variation in monthly sales.
* It captured multiple business drivers simultaneously.
* It provided stronger support for business decision-making.

---

## Business Recommendation

The analysis suggests that leadership should focus primarily on:

* Marketing effectiveness
* Increasing customer footfall
* Maintaining high inventory availability

These factors showed the strongest association with monthly sales performance.

Variables with weaker statistical evidence should not be over-interpreted without additional analysis.

---

## Assumptions and Limitations

The regression model has several limitations:

* It does not capture competitor activity.
* Seasonal demand fluctuations are not included.
* Local economic conditions may influence store performance.
* Customer demographics are not included in the analysis.

Regression analysis identifies associations but does not automatically prove causation.

---

## Residual Analysis

Residual analysis was performed to compare actual sales with predicted sales.

The analysis identified stores where the model under-predicted and over-predicted sales performance and highlighted opportunities for future model improvement.

---

## Screenshots Included

The repository contains the following screenshots:

* simple_regression_output.png
* multiple_regression_output.png
* residuals_preview.png
* model_comparison_preview.png

These screenshots provide evidence of the regression analysis and model evaluation process.

---

## Repository Structure

```text
part3_regression_insights/
├── data/
│   └── business_regression_data.xlsx
├── analysis/
│   ├── regression_workbook.xlsx
│   ├── model_comparison.md
│   └── residual_analysis.md
├── outputs/
│   ├── regression_summary.xlsx
│   ├── final_recommendation.md
│   └── model_equations.md
├── screenshots/
│   ├── simple_regression_output.png
│   ├── multiple_regression_output.png
│   ├── residuals_preview.png
│   └── model_comparison_preview.png
└── README.md
```

## Conclusion

The project demonstrates how regression analysis can help retail businesses understand sales drivers and support data-driven decision-making.

The findings indicate that marketing investment, customer footfall, and inventory availability are the strongest business factors associated with monthly sales performance.
