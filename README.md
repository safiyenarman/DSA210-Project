# DSA210-Term-Project

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
- **Sources:**  
  - Happiness data will be collected from the World Happiness Report dataset on Kaggle.  
  - SDG data will be obtained from the Sustainable Development Report dataset on Kaggle.  
- **Consistency:**  
  - Only countries with data available for both happiness and SDG ranks for each year between 2015 and 2022 will be included.  
  - Missing data will be addressed using appropriate imputation methods or by excluding countries with significant gaps.

### 2. Data Preparation and Cleaning
- **Merging:**  
  - The two datasets will be merged based on the country and year fields.  
- **Handling Missing Values:**  
  - Missing ranks will be addressed using mean or median imputation if gaps are minor.  
  - Countries with extensive missing data will be excluded.  
- **Normalization:**  
  - Rank data may be normalized to ensure comparability between happiness and SDG ranks.

### 3. Exploratory Data Analysis (EDA)
- **Visualization:**  
  - Using visualization techniques to illustrate correlations and trends.
- **Statistical Analysis:**  
  - Correlation coefficients to assess the strength and direction of relationships.  
  - Clustering analysis to group countries based on similar patterns in happiness and SDG progress.

### 4. Regression Analysis
- **Goal:**  
  - To quantify the impact of SDG progress on happiness ranks.  
- **Methods:**  
  - Linear regression to model the relationship between SDG ranks and happiness ranks.  

### 5. Reporting and Insights
- **Key Findings:**  
  - Summarize how SDG progress correlates with happiness ranks.  
  - Highlight which SDGs (e.g., health, education, equality) have the most significant impact on happiness.  
- **Recommendations:**  
  - Suggestions for policymakers on prioritizing SDGs to enhance happiness.  

By following this plan, I aim to uncover actionable insights into how sustainable development efforts can effectively boost happiness levels globally.
