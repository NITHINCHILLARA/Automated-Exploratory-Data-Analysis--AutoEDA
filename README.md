# Automated EDA (Exploratory Data Analysis)
## Objective: 
Replace manual data profiling with one-line AI summaries to identify data quality issues instantly.
● Key Concept: AutoEDA allows you to visualize distributions, correlations, and missing values without writing individual plots for every column.
● Documentation: ydata-profiling Documentation
● Dataset Recommendation: Kaggle E-commerce Sales Data
## Script to Execute:
## Python
import pandas as pd
from ydata_profiling import ProfileReport
### Load your dataset
df = pd.read_csv("Ecommerce_Sales_Prediction_Dataset.csv")
### Generate the AI-powered report
profile = ProfileReport(df, title="Weekly Audit Report", explorative=True)
### Export to HTML for stakeholder review
profile.to_file("AutoEDA_Report.html")
### Final Auto EDA Report Link :
https://nithinchillara.github.io/Auto-EDA-Report/
