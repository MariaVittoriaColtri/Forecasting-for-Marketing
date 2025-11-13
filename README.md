# Sales Forecasting Using Multivariate Linear Regression 

<br>

## Project Overview <br>

This project implements a multivariate linear regression approach to quantify the influence of three advertising channels (TV, Radio, and Newspaper) on weekly sales. The main goal is to accurately measure channel effectiveness, validate the model, and provide evidence-based recommendations to optimize marketing spend. The approach draws upon theoretical foundations and practical methods from An Introduction to Statistical Learning: With Applications in Python (James et al., 2023). <br><br>

## Table of Contents <br>

1. Dataset Description
2. Data Import and Transformation
3. Exploratory Data Analysis (EDA)
4. Correlation Analysis
5. Model Training and Inference
6. Model Validation Using Excel
7. Results and Visualizations
8. Recommendations for the Marketing Team <br><br>

## Dataset Description <br>

The dataset contains 183 weekly observations with complete data on advertising budgets and sales:
• TV advertising budget: average 148.18 (std dev 86.33)
• Radio advertising budget: average 23.52 (std dev 14.99)
• Newspaper advertising budget: average 30.47 (std dev 21.82)
• Weekly sales volume (target): average 14.15 (std dev 5.25)

No missing or inconsistent data was found, ensuring high data quality for analysis. <br><br>

## Data Import and Transformation <br>

The dataset was imported and transformed with emphasis on data quality standards. Checks confirmed zero missing values and ensured no inconsistencies, guaranteeing reliable input for comprehensive analysis and modeling. <br><br>

## Exploratory Data Analysis (EDA) <br>

Exploratory analysis assessed relationships between predictors and sales as well as non-predictive variables. Correlation metrics were computed and visualized to understand underlying patterns, laying a solid statistical foundation for model development. <br><br>

## Correlation Analysis <br>

Pearson correlation analysis revealed a strong positive linear relationship between sales and advertising spend on TV (approximately 0.78) and Radio (approximately 0.58). In contrast, advertising spend on Newspaper demonstrated a weak linear association with sales (approximately 0.05), indicating minimal influence.

Multicollinearity diagnostics further confirmed that each predictor contributes independently to the model without significant redundancy, supporting the robustness of the inference. <br><br>

## Model Training and Inference <br>

The data was split into training and test sets with a 70% / 30% ratio, yielding 128 observations for training and 55 for testing. This split ensured sufficient data to fit the model and robust assessment of generalization on unseen data.

The multivariate linear regression model identified:
• Significant positive effects of TV and Radio advertising on sales (p < 0.001)
• Insignificant impact of Newspaper advertising
• Explained variance (R²) of approximately 0.88
• Mean Squared Error (MSE) on test data around 4.4, confirming precise predictive performance <br><br>

## Model Validation Using Excel <br>

Regression coefficients were manually applied in Excel to replicate predictions on a subset of weeks. Calculated sales closely echoed actual sales, verifying the correctness of model calculations and enhancing transparency and confidence.

Excel Coefficients Table:

Figure 1: Weekly ice tea sales dataset (first 20 weeks of data).

Figure 2 : Regression coefficients used for manual prediction in Excel.

Figure 3 : Example of manual predicted revenue calculation for Week 1 and Week 2.

Figure 4 : Comparison between predicted and actual sales
The chart compares predicted (orange line) and actual sales (blue bars) over 52 weeks.
The close alignment confirms strong model accuracy in capturing seasonal and marketing effects.
Peaks around weeks 25–35 reflect higher sales driven by holidays and social media campaigns. <br><br>

## Results and Visualizations <br>

Analyses are complemented by:
• A heatmap of the correlation matrix visualizing variable relationships.
• Line plots comparing real versus predicted sales over the test period.

These visualizations effectively communicate model accuracy and channel impacts. <br><br>

## Recommendations for the Marketing Team <br>

• Increase investment in TV and Radio channels as these have the strongest positive impact on sales.
• Reallocate part of the Newspaper advertising budget towards more ROI-efficient channels.
• Maintain stable pricing strategies since price fluctuations negatively affect sales volume; discounts should be used carefully.
• Align major campaigns with peak seasonal periods, such as holidays, to maximize sales effectiveness.
• Update the model using new data to continuously refine marketing budget allocation and media effectiveness insights. <br>

