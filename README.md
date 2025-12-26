Student Performance Prediction – Machine Learning Semester Project
Python
scikit-learn
Jupyter
License: MIT
Project Overview
This repository contains the final semester project for the Machine Learning course taught by Professor Dr. Abdul Razaque, PhD & Postdoc.
The objective is to predict students' mathematics exam scores (regression task) using demographic and study-related features from the well-known "Students Performance in Exams" dataset on Kaggle.
The project implements a complete machine learning pipeline:

Data loading and initial exploration
Data cleaning and preprocessing
Feature engineering
Exploratory Data Analysis with visualizations
Baseline model: Linear Regression
Advanced model: Random Forest Regressor with hyperparameter tuning (GridSearchCV)
Model evaluation and comparison
Result interpretation and practical insights

Key finding: Random Forest significantly outperforms the baseline, confirming that test preparation courses and socioeconomic factors (parental education, lunch type) have strong influence on performance.
Dataset
Source: Students Performance in Exams – Kaggle
Author: spscientist (2018)
Size: 1,000 rows × 8 columns
License: CC0 (Public Domain)
Features:

gender – male/female
race/ethnicity – group A to E (anonymized)
parental level of education – from "some high school" to "master's degree"
lunch – standard / free/reduced (socioeconomic proxy)
test preparation course – completed / none
reading score – 0–100
writing score – 0–100
math score – target variable (0–100)

Note: The original CSV file is not included due to Kaggle terms. Download StudentsPerformance.csv from the link above and place it in the repository root.
Generated Files
Running the notebook automatically creates:

original_dataset.csv – untouched copy of raw data
cleaned_dataset.csv – preprocessed version with engineered features

Project Structure
textstudent-performance-prediction/
├── finalProject.ipynb          # Main Jupyter notebook with full code and analysis
├── StudentsPerformance.csv     # Download from Kaggle and add here
├── original_dataset.csv        # Generated automatically
├── cleaned_dataset.csv         # Generated automatically
├── README.md                   # This file
└── LICENSE                     # MIT License
Requirements
Python 3.10 or higher.
Required libraries (install via pip):
textpip install pandas numpy matplotlib seaborn scikit-learn
No additional packages needed.
How to Run

Clone the repository:textgit clone https://github.com/your-username/student-performance-prediction.git
cd student-performance-prediction
Download the dataset:
Go to the Kaggle link above
Download StudentsPerformance.csv
Place it in the project root

Launch Jupyter:textjupyter notebookortextjupyter lab
Open finalProject.ipynb and run all cells sequentially.

The notebook will load the data, perform preprocessing, display visualizations, train models, and show results.
Key Results























ModelRMSEMAER²Linear Regression (Baseline)~13.5~10.7~0.21Random Forest (Improved)~10.8~8.4~0.46
Main insights:

Random Forest clearly outperforms the baseline.
Most influential features: reading/writing scores, test preparation completion, parental education, lunch type.
Practical recommendation: prioritize test preparation courses and targeted support for students from lower socioeconomic backgrounds.

Visualizations Included

Descriptive statistics
Score distributions (histograms)
Correlation heatmap
Boxplots by categorical features (gender, preparation, lunch, parental education)
Actual vs. Predicted scatter plot (model comparison)
Feature importance bar plot (Random Forest)

Possible Extensions

Experiment with gradient boosting models (XGBoost, LightGBM, CatBoost)
Multi-output regression to predict all three scores simultaneously
Advanced feature engineering (e.g., average score, gaps between subjects)
Fairness analysis to check for bias in demographic features
Deploy as a web application (Streamlit or Flask)

Contributing
Contributions are welcome. Feel free to:

Open issues for bugs or suggestions
Submit pull requests with new models, visualizations, or improvements

License
This project is licensed under the MIT License – see the LICENSE file for details.
The dataset is subject to its original Kaggle license and terms of use.
Submitted by:
Amina Kabidesh
Nuray Bolat
Course: Machine Learning Semester Project
Date: December 2025
Thank you for checking out our project!
