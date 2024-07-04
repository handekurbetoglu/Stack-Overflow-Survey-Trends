# Project Overview

This project provides an in-depth analysis of the Stack Overflow Developer Survey dataset, focusing on global developer trends in roles, education, and compensation. The analysis reveals critical insights into the developer community, highlighting trends in developer roles, educational backgrounds, and compensation structures.

## Files and Directories
developer_dataset.csv: Dataset containing the survey data used in this analysis.
stack_overflow_survey_analysis.ipynb: Jupyter notebook containing the full analysis.
read_me.md: This project overview and instructions.


## Analysis Methodology

### 1. Data Collection
Dataset: developer_dataset.csv, which contains developer survey responses gained from stackoverflow.

### 2. Data Cleaning
Missing Data Removal: Columns with over 60% missing values were removed to enhance data quality.
Filtering Rows: Rows with missing values in crucial columns (Employment, DevType) were removed.

### 3. Feature Engineering
Developer Roles Analysis:
New binary columns (BackEnd, FrontEnd, FullStack, Mobile, Admin, Data Scientist) were created based on DevType.
Education Analysis:
Missing values in UndergradMajor were filled using backward fill (bfill).
New binary columns representing educational backgrounds were created (SocialScience, NaturalScience, ComSci, OtherEng, Data, NoMajor).

### 4. Years of Experience & Compensation
Iterative Imputation: Missing values in YearsCodePro and ConvertedComp were filled using IterativeImputer.
Binning Years of Experience: YearsCodePro was binned into quartiles for analysis.
Boxplot Visualization: Relationships between experience levels and compensation were visualized.

### 5. Developer Salaries Analysis
Developer Type Flags: Binary flags for developer types were created.
Average Salary Calculation: Mean salaries were calculated and visualized by developer role.


## Key Insights

### Developer Distribution by Country:
Developer roles vary significantly across countries, with regional preferences for specific roles.
Popular Developer Roles:
Backend, Frontend, and Full Stack developers are the most common roles globally.

### Educational Background Trends:
Computer Science remains the most popular educational background, followed by engineering.
Years of Experience & Compensation:
Compensation increases significantly with years of professional coding experience.

### Average Salaries by Developer Type:
Data Scientists and Full Stack Developers tend to have higher average salaries.

## Conclusions and Recommendations

### Targeted Educational Outreach:
Encourage educational institutions to focus on computer science and data science programs due to the growing demand.

### Professional Development:
Developers should pursue continuous learning, especially in data science and full-stack development.

### Global Collaboration:
Companies should leverage remote work opportunities to tap into global developer talent.

## Further Analysis:
Investigate correlations between programming languages and compensation.
Study developer satisfaction trends based on role and salary.
Instructions to Reproduce Analysis

## Requirements:
Python 3.x
Jupyter Notebook
Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

## Setup:
Clone or download this repository.
Install required libraries:
pip install pandas numpy matplotlib seaborn scikit-learn

Launch Jupyter Notebook:
jupyter notebook
Open stack_overflow_survey_analysis.ipynb and execute cells sequentially.
