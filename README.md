# PowerCo-Customer-Churn-Analysis-EDA



![image alt]()

# Overview

This project analyzes customer churn for PowerCo using data science
techniques to investigate whether price sensitivity may be
associated with customers switching energy providers.
The project follows a structured data science workflow:
Business Understanding → Exploratory Data Analysis → Feature
Engineering → Modeling & Evaluation → Insights & Recommendations
The goal is to identify useful churn-related patterns and build a
machine learning model that can help PowerCo better identify customers
at risk of churn.
Business Problem
PowerCo wanted to investigate the hypothesis that customers are becoming
more price-sensitive and may be switching to lower-cost energy
providers.
The analysis therefore considers price-related factors alongside other
potential churn drivers such as:
- Customer consumption
- Contract and renewal information
- Customer tenure
- Product relationships
- Discounts
- Historical pricing
- Customer characteristics
# Tools & Methods

Tools

- Python
- Google Colab / Jupyter Notebook
- Pandas & NumPy -- data manipulation and analysis
- Matplotlib & Seaborn -- data visualization
- Scikit-learn -- machine learning

# Methods

- Data cleaning and validation
- Exploratory Data Analysis (EDA)
- Descriptive statistics
- Distribution and outlier analysis
- Correlation analysis
- Feature engineering
- Random Forest classification
- Model evaluation using Accuracy, Precision, Recall, F1 Score and
  ROC-AUC

# Project Workflow

1. Exploratory Data Analysis
Analyzed: - Data types and structure - Missing values and duplicates -
Descriptive statistics - Numerical and categorical distributions - Churn
distribution - Customer and pricing patterns - Differences between
churned and retained customers
2. Feature Engineering
Created meaningful features including: - Customer lifecycle and renewal
features - Consumption vs forecast ratios - Product/customer value
indicators - Annual and 6-month price change features - Absolute price
change - Price change acceleration - Overall forecast price indicators -
Discount indicators
3. Modeling
A Random Forest Classifier was trained to predict customer churn.
A stratified train-test split was used, with balanced class weights to
account for the relatively small proportion of churned customers.
4. Evaluation
  Metric         Result
  Churn rate       9.7%
  Accuracy        91.0%
  Precision       84.2%
  Recall           9.0%
  F1 Score        16.3%
  ROC-AUC         70.0%
Because churn is a minority class, accuracy alone is not sufficient.
Recall and F1 Score are particularly important because missing customers
who are likely to churn can reduce the usefulness of a retention
strategy.
The model shows some predictive signal, but its low recall means further
improvement would be needed before relying on it as a primary
churn-retention tool.

# Key Insights

- Customer churn is relatively infrequent, with approximately 9.7%
  of customers churning.
- Price-related features were specifically engineered to investigate
  the price-sensitivity hypothesis.
- Customer consumption, tenure, product relationships and
  pricing-related variables provide useful dimensions for
  understanding churn.
- The Random Forest model achieved 91% accuracy, but its 9%
  recall shows that it identifies only a small proportion of actual
  churners.
- Model performance should therefore be improved before using
  predictions for large-scale retention decisions.

# Recommendations

- Improve churn detection by focusing on recall, rather than
  accuracy alone.
- Further investigate price-related behavior alongside non-price churn
  drivers.
- Test additional classification approaches and model tuning.
- Use customer segmentation to identify groups with different churn
  patterns.
- Once model performance improves, use churn-risk predictions to
  support targeted retention strategies.

# Project Structure

PowerCo-Customer-Churn-Analysis/
│
├── data/
│   └── Project datasets
│
├── notebooks/
│   ├── EDA.ipynb
│   ├── Feature_Engineering.ipynb
│   └── Modeling_and_Evaluation.ipynb
│
├── presentation/
│   └── Executive_Summary.pdf
│
└── README.md

# Conclusion

This project demonstrates an end-to-end data science approach to
understanding and predicting customer churn. The analysis provides an
initial assessment of the price-sensitivity hypothesis, develops
useful churn-related features, and evaluates a Random Forest model.
The results indicate that the current model has predictive signal but
requires further improvement, particularly in identifying actual
churners, before it can be confidently used for customer retention
decisions.
Thank you for taking the time to check out this project! Your interest,
feedback, and contributions mean a lot. If you have any suggestions,
feel free to share.
Don't forget to ⭐ this repository if you found it helpful --- it really
helps others find it too.
Happy coding
