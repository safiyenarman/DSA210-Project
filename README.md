#SDG and World Happiness Rankings ML Project

## Project Idea
In this project, I will analyze the relationship between the Sustainable Development Goals (SDGs) rankings and World Happiness Rankings for countries between 2015 and 2022. The goal is to explore how progress towards sustainable development influences the perceived happiness of populations worldwide. I aim to identify patterns and correlations that might suggest that improvements in areas such as health, education, and economic equality (as outlined by the SDGs) are associated with higher happiness levels.
##

## Motivation 
Sustainable Development Goals (SDGs) aim to make the world fairer and healthier for everyone. Happiness and well-being are key parts of sustainable living, but we still don't fully understand how progress in sustainability directly affects people's happiness. Studying this connection can help governments and organizations choose actions that improve both sustainability and happiness.
##

## Description of Dataset
### 1. Happiness Data
- **Source:** [World Happiness Report on Kaggle](https://www.kaggle.com/datasets/mathurinache/world-happiness-report)
- **Key Variables:**
  - **Country:** Name of the country.
  - **Happiness Rank:** The rank of each country based on the average happiness scores derived from factors such as GDP per capita, social support, life expectancy, freedom to make life choices, generosity, and perceptions of corruption.
  - **Year:** Data available for each year between 2015 and 2022.

### 2. SDGs Data
- **Source:** [Sustainable Development Report on Kaggle](https://www.kaggle.com/datasets/sazidthe1/sustainable-development-report/data)
- **Key Variables:**
  - **Country:** Name of the country.
  - **Overall SDG Rank:** The rank of countries based on their progress towards achieving the 17 Sustainable Development Goals.
  - **Year:** Data available for each year between 2015 and 2022.

### 3. Merged Dataset
- **Country:** To match data points accurately, I will use country names as the primary key.
- **Time:** I will focus on the years from 2015 to 2022, ensuring that the data is consistent across both datasets.
- **Overall SDG Rank:** This variable will indicate a country’s progress towards sustainability.
- **Happiness Rank:** This variable will represent the perceived well-being of populations.
##

## Plan
### 1. Data Collection
- I will use datasets from the World Happiness Report and the Sustainable Development Report, both available on Kaggle.
To ensure consistency, I will include only countries with complete data between 2019 and 2022, excluding those with extensive missing values.

### 2. Data Preparation and Cleaning
- The datasets will be merged using country and year as key fields.
For modeling purposes, I will retain only countries in the top and bottom SDG score ranges, removing those in the middle range.
Missing values will be handled by dropping incomplete rows to ensure data quality.


### 3. Exploratory Data Analysis (EDA)
- I will apply various visualization techniques (boxplots, histograms, scatter plots, and line graphs) to explore the trends and distributions in the data.
I will also calculate correlation coefficients to investigate the strength of the relationship between SDG and happiness scores.
Initial insights will guide the modeling strategy and help frame relevant hypotheses.


### 4. Hypothesis Testing
- I will test whether the relationship between SDG Scores and Happiness Scores is statistically significant using Pearson correlation and Welch’s T-tests.
This will help validate whether higher SDG performance is associated with higher happiness levels.


### 5. Machine Learning Modeling
- To predict SDG performance categories, I will frame a binary classification problem using Happiness Score and Year as features.
I plan to implement and compare Logistic Regression, Random Forest, and XGBoost classifiers.
Model performance will be evaluated based on metrics like accuracy, recall, specificity, and AUC.


### 5. Reporting and Insights
- The final report will summarize key findings and identify whether sustainable development significantly aligns with national well-being.
I will also reflect on the policy implications, suggesting how investment in SDGs could help increase national happiness.
Future work may involve adding more predictors or extending the time range for a deeper analysis.


By following this plan, I aim to uncover actionable insights into how sustainable development efforts can effectively boost happiness levels globally.
