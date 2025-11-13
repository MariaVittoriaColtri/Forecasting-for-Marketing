# Sales Forecasting Using Multivariate Linear Regression

<br>

## Introduction <br>

This project implements a multivariate linear regression approach to quantify the influence of three advertising channels (TV, Radio, and Newspaper) on weekly sales. The approach draws upon theoretical foundations and practical methods from An Introduction to Statistical Learning: With Applications in Python (James et al., 2023). <br><br>

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
- TV advertising budget: average 148.18 (std dev 86.33) <br>
- Radio advertising budget: average 23.52 (std dev 14.99) <br>
- Newspaper advertising budget: average 30.47 (std dev 21.82) <br>
- Weekly sales volume (target): average 14.15 (std dev 5.25) <br> <br>
No missing or inconsistent data was found, ensuring high data quality for analysis. <br><br>

## Data Import and Transformation <br>

The dataset was imported and transformed with emphasis on data quality standards. Checks confirmed zero missing values and ensured no inconsistencies, guaranteeing reliable input for comprehensive analysis and modeling. <br><br>

## Exploratory Data Analysis (EDA) <br>

Exploratory analysis assessed relationships between predictors and sales as well as non-predictive variables. Correlation metrics were computed and visualized to understand underlying patterns, laying a solid statistical foundation for model development. <br><br>

## Correlation Analysis <br>

Pearson correlation analysis revealed a strong positive linear relationship between sales and advertising spend on TV (approximately 0.78) and Radio (approximately 0.58). In contrast, advertising spend on Newspaper demonstrated a weak linear association with sales (approximately 0.05), indicating minimal influence.

Multicollinearity diagnostics further confirmed that each predictor contributes independently to the model without significant redundancy, supporting the robustness of the inference. <br><br>

## Model Training and Inference <br>

The data was split into training and test sets with a 70% / 30% ratio, yielding 128 observations for training and 55 for testing. This split ensured sufficient data to fit the model and robust assessment of generalization on unseen data. <br>
The multivariate linear regression model identified:
- Significant positive effects of TV and Radio advertising on sales (p < 0.001) <br>
- Insignificant impact of Newspaper advertising <br>
- Explained variance (R²) of approximately 0.88 <br>
- Mean Squared Error (MSE) on test data around 4.4, confirming precise predictive performance <br> <br><br>

## Model Validation Using Excel <br>

Regression coefficients were manually applied in Excel to replicate predictions on a subset of weeks. Calculated sales closely echoed actual sales, verifying the correctness of model calculations. <br>


<img width="532" height="379" alt="Screenshot 2025-10-25 221050" src="https://github.com/user-attachments/assets/92a1817d-88c9-4a83-9981-734327adad28" />


Figure 1: Weekly ice tea sales dataset (first 20 weeks of data). <br>


<img width="193" height="156" alt="Screenshot 2025-10-25 222524" src="https://github.com/user-attachments/assets/6469f1ee-93d5-41f0-9420-ab423b7d6749" /> 


Figure 2 : Regression coefficients used for manual prediction in Excel. <br> 


<img width="1186" height="624" alt="Screenshot 2025-11-13 174558" src="https://github.com/user-attachments/assets/eaf15dc7-1788-4efc-b614-d6457b64ed86" /> 

Figure 3 – Weekly ice tea sales compared with model predictions and variable contributions. <br> 

This chart shows the weekly ice tea sales compared with the model’s predictions. The orange line represents actual revenue, while the bars reflect the contribution of each variable in the regression formula. The overall alignment between the two trends confirms that the model follows the real sales pattern closely across the year.


## Results and Visualizations <br>

This analysis is reinforced by: <br>
• A heatmap of the correlation matrix visualizing variable relationships. <br> 
• Line plots comparing real versus predicted sales over the test period. <br> 

<img width="698" height="630" alt="Screenshot 2025-11-11 192014" src="https://github.com/user-attachments/assets/235f4793-6cbe-4503-9ab7-4a877953c5d7" /> <br> <br>
<img width="755" height="513" alt="Screenshot 2025-11-13 173717" src="https://github.com/user-attachments/assets/e65cb22e-9b1f-4d5a-8bb7-eb3b6fbe23ef" /> 

The correlation matrix highlights the linear relationships between all variables, showing strong positive correlations between Revenue and channels such as Search, Newspaper, and Temperature, while Price_delta displays a weak negative effect. At the same time, the Actual vs Predicted line chart shows that the model’s predicted sales closely follow the real observations, indicating that the OLS regression reflects the main sales patterns with good accuracy and limited deviation. <br>  


## Recommendations for the Marketing Team <br>

• Increase investment in TV and Radio channels as these have the strongest positive impact on sales. <br>
• Reallocate part of the Newspaper advertising budget towards more ROI efficient channels. <br>
• Maintain stable pricing strategies since price fluctuations negatively affect sales volume; discounts should be used carefully. <br>
• Align major campaigns with peak seasonal periods, such as holidays, to maximize sales effectiveness. <br>
• Update the model using new data to continuously refine marketing budget allocation and media effectiveness insights. <br> <br>
