# HR Attrition Analysis and Prediction

## Executive Summary

### **Objective:**

The **HR Attrition Analysis and Prediction** project aims to help organizations understand and address employee turnover. By analyzing employee data, including factors like age, job satisfaction, income, and overtime, the project identifies key drivers of attrition. Additionally, predictive models were developed to forecast employee turnover, enabling HR teams to proactively manage retention strategies.

### **Context:**

To conduct this analysis, the project used R, a powerful statistical programming language, and its associated libraries for data visualization, statistical testing, and predictive modeling. The analysis utilized a dataset containing detailed employee information, including demographic details and job-related variables. Key techniques employed included Exploratory Data Analysis (EDA), hypothesis testing, and machine learning models to predict which employees are at risk of leaving.

## Requirements

- R (version 4.0 or later)
- Required R packages:
  - `shiny`
  - `ggplot2`
  - `plotly`
  - `caret`
  - `randomForest`
  - `DataExplorer`
  - `reshape2`

## Installation

1. Clone the repository:
```bash
   git clone https://github.com/IshwaryaKeerthivasan/HR-Employee-Attrition.git
```

2. Open the project folder and install the necessary R packages by running the following in R:
```bash
install.packages(c("shiny", "ggplot2", "plotly", "caret", "randomForest", "DataExplorer", "reshape2"))
```

## Features

- **Dynamic Visualizations**: Explore how factors like age, income, job satisfaction, and overtime affect employee attrition.
- **Extensive EDA**: Comprehensive data analysis to uncover key trends and relationships in the dataset.
- **Outlier Detection**: Identifies outliers in data like age and income, which may provide valuable insights into retention.
- **Statistical Analysis**: Hypothesis tests (e.g., Chi-squared, ANOVA) to examine correlations and significant factors affecting attrition.
- **Predictive Modeling**: Uses machine learning algorithms, such as logistic regression and random forests, to predict employee attrition and identify high-risk employees.
- **Machine Learning Insights**: Provides actionable insights from model results, helping HR teams prioritize interventions for employees most likely to leave.
- **Interactive Interface**: Hover over visualizations for dynamic tooltips and real-time insights.


## Business Problem

### Problem Identification:
The primary challenge addressed in this project is the high employee attrition rate in specific departments, which can negatively impact organizational performance. By understanding the underlying factors contributing to employee turnover, HR teams can develop targeted strategies to improve retention and reduce attrition.

### Business Impact:
High attrition rates result in increased recruitment and training costs, reduced employee morale, and decreased productivity. By addressing these issues, organizations can enhance employee satisfaction, reduce turnover, and ultimately improve organizational stability and performance.

## Methodology

### Data Cleaning & Transformation:
- **Handling Missing Data**: Missing values were addressed by removing rows with incomplete information.
- **Categorical Data**: Categorical variables were converted into factors to enable meaningful analysis.
- **Zero Variance**: Columns with no variation were removed to simplify the dataset and focus on relevant features.
- **Outlier Detection**: Outliers in critical variables like age and income were identified and reviewed for their impact on the analysis.

### Analysis Techniques:
- **Exploratory Data Analysis (EDA)**: A deep dive into the dataset using visualizations to understand the relationships between key factors, such as age, income, overtime, and attrition.
- **Statistical Analysis**: Conducted hypothesis tests (e.g., Chi-squared, ANOVA) to identify significant factors contributing to attrition.
- **Predictive Modeling**: Machine learning techniques, including logistic regression and random forests, were used to predict the likelihood of employee attrition based on various factors, enabling HR teams to identify at-risk employees and prioritize retention efforts.

## Skills

### Tools, Languages, & Software:
- **Languages**: R
- **Libraries/Tools**: `shiny`, `ggplot2`, `plotly`, `caret`, `randomForest`, `DataExplorer`, `reshape2`
- **Platform**: RStudio or Shiny Server to run the interactive dashboard

## Results & Business Recommendation

### Business Impact:
The findings from the analysis provided actionable insights that HR teams can use to reduce attrition. For example, departments with high overtime rates were found to experience more turnover, while younger employees (ages 25–35) were more likely to leave. By focusing on improving job satisfaction and addressing specific pain points within departments, organizations can increase retention.

### Insights:
- **Age Factor**: Younger employees (ages 25-35) tend to have higher attrition rates, indicating a need for tailored retention strategies for this group.
- **Overtime**: Employees working overtime are more likely to leave, particularly in high-pressure departments. Addressing workload balance can improve retention.
- **Job Satisfaction**: Low job satisfaction was found to correlate with higher turnover. Improving work culture and employee engagement can be pivotal in reducing attrition.

### Predictive Modeling Findings:
- **Logistic Regression**: The logistic regression model revealed that variables like **Job Satisfaction**, **Overtime**, and **Income** are significant predictors of attrition. Employees with low satisfaction and higher overtime hours are more likely to leave the organization. The model achieved an accuracy of approximately 80% in predicting employee attrition.
- **Random Forest Model**: The random forest model, which uses multiple decision trees to improve prediction accuracy, indicated that **Overtime** and **Job Role** were among the most important factors affecting attrition. The random forest model achieved an accuracy of 85%, and it provided a better understanding of the complex, non-linear relationships in the data.
- **Feature Importance**: Both models highlighted **Overtime** and **Job Satisfaction** as critical features influencing employee retention. These findings can guide HR teams to prioritize interventions in these areas to minimize turnover.

### Visualizations:
Interactive visualizations were developed to illustrate the relationships between key factors and attrition. These visualizations provide HR teams with dynamic tools to explore the data and understand how different variables contribute to turnover.

## Next Steps

### Future Work:
- **Demographic Expansion**: The analysis could be extended to include additional demographic factors, such as education level, tenure, and performance metrics.
- **Enhanced Predictive Models**: Future improvements could involve refining predictive models by incorporating more features or experimenting with other machine learning algorithms like decision trees or XGBoost.
- **Dashboard Improvements**: Enhancing the dashboard with more interactive features and real-time filters would allow HR teams to explore the data in more depth and gain deeper insights.
