# Capstone-Project-20.1-Initial-Report-and-Exploratory-Data-Analysis-EDA-

## The Initial Report and Exploratory of My Dataset

### Dataset Information:
The dataset is sourced from an AI-powered job market insights platform, providing anonymized data on job roles, salaries, industries, and adoption of AI across organizations.

### Business Understanding
What is the AI-Powered Job Market Study?
The future of the job market is influenced significantly by Artificial Intelligence (AI). Key aspects include:

###  Understanding which industries are leading in AI adoption.
Examining salary trends across different roles, industries, and risk levels.
Evaluating the relationship between AI adoption and remote work opportunities.
This study provides valuable insights to help businesses, policymakers, and job seekers make informed decisions.

### Why Choose AI for this Analysis?
AI allows for data-driven insights, including:

Predicting future trends in job roles and salaries.
Assessing automation risks for specific roles.
Analyzing correlations between job growth projections and salaries.
By leveraging machine learning and visualization tools, we aim to extract actionable insights for strategic planning.

### Source:
AI-Powered Job Market Insights Dataset (from Kaggle:https://www.kaggle.com/datasets/uom190346a/ai-powered-job-market-insights)

### Data Understanding
<pre> Dataset Characteristics: Tabular data Domain: Job Market Analysis Features: Mixed (Categorical, Numerical) Missing Values? No </pre>
### Attributes Information:
The dataset includes the following columns:

Job_Title: The title of the job role.
Industry: The industry of the job.
Company_Size: The size of the company.
Location: Job location.
AI_Adoption_Level: The level of AI adoption in the company.
Automation_Risk: The risk of automation for the role.
Required_Skills: Skills required for the job.
Salary_USD: Annual salary in USD.
Remote_Friendly: Whether the job supports remote work.
Job_Growth_Projection: Projected growth for the role.
### Directory Structure
<pre> ├── data │ ├── ai_job_market_insights.csv ├── models │ ├── job_market_trends.ipynb │ ├── ai_job_predictions.json ├── presentation │ ├── Job_Market_Analysis.pptx </pre>
### Data Preparation and Visualization
<pre> Code Language: Python Libraries Used: Pandas, Numpy, Matplotlib, Seaborn </pre>
Data Cleaning, Processing, and Modeling
<pre> Code Language: Python Libraries Used: Pandas, Seaborn, Matplotlib </pre>

## Modeling and Classification:
### Objectives:
1.Classify Industries:

Predict the industry type (Manufacturing, Technology, Education) based on salary levels and risk factors.
Use salary ranges (Low, Medium, High) as predictors.

2.Modeling Techniques:

Logistic Regression: Efficient for binary and multi-class classification.
Random Forest Classifier: Robust and flexible for industry prediction.
### Data Preparation:
Feature Engineering:
Created Salary_Range based on salary distribution.
Filtered top three industries by frequency.
Used dummy encoding for Salary_Range.
Training-Test Split:
80% training, 20% testing.
Standard scaling applied to numerical features.
### Results:
Logistic Regression:

Accuracy: 73%
Best Hyperparameter (C): 1.0
Confusion Matrix shows balanced predictions but slight misclassification between Technology and Manufacturing.
Random Forest:

Accuracy: 82%
Best Parameters: 200 estimators, max depth of 10.
Outperformed logistic regression, especially in distinguishing Manufacturing from Education.
### Visualizations:
Confusion Matrices:
Highlighted misclassifications and model strengths.
Feature Importances (Random Forest):
High correlation between Salary_Range and industry prediction.
## Process Summary:
The project successfully analyzed AI adoption trends in the job market and classified industries based on salary ranges.

### Key Takeaways:
Manufacturing, Technology, and Education are the leading industries in AI adoption.
High automation risk correlates with lower salaries, especially in roles with repetitive tasks.
Random Forest Classifier provides the most accurate predictions for industry classification.
### Future Work:
Incorporate additional features like Required_Skills and Location to refine predictions.
Use advanced models (e.g., Gradient Boosting, Neural Networks) for salary prediction.
How to Use:
