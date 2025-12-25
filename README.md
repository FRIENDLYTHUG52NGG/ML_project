#Student Performance Prediction – Machine Learning Semester Project
Python
scikit-learn
License
Jupyter
📌 Project Description
This repository contains the final semester project for a Machine Learning course. The goal is to predict students' math scores based on demographic and academic preparation features using the famous "Students Performance in Exams" dataset from Kaggle.
The project covers the full machine learning pipeline:

Data loading and initial exploration
Data cleaning and preprocessing
Feature engineering
Exploratory Data Analysis (EDA) with visualizations
Baseline model (Linear Regression)
Advanced model (Random Forest Regressor) with hyperparameter tuning
Model evaluation and comparison
Interpretation of results

📊 Dataset

Source: Students Performance in Exams – Kaggle
Filename: StudentsPerformance.csv (download from Kaggle and place in the root folder)
Size: 1,000 rows × 8 columns
Features:
gender – student's gender (male/female)
race/ethnicity – ethnicity group (group A to E)
parental level of education – parents' highest education
lunch – type of lunch (standard / free/reduced)
test preparation course – whether the student completed a preparation course
math score – target variable (0–100)
reading score – additional score
writing score – additional score


Note: The dataset is not included in the repository due to Kaggle licensing. You must download it yourself.
🛠️ Generated Files
Running the notebook will create:

original_dataset.csv – untouched copy of the raw data
cleaned_dataset.csv – cleaned version with engineered features

📋 Project Structure
text.
├── finalProject.ipynb              # Main Jupyter notebook with full analysis
├── StudentsPerformance.csv         # ← You need to add this (download from Kaggle)
├── original_dataset.csv            # ← Generated
├── cleaned_dataset.csv             # ← Generated
├── README.md                       # This file
└── LICENSE                         # MIT License (optional)
⚙️ Requirements
All required packages are listed in the notebook, but here is the full list:
Bashpip install pandas numpy matplotlib seaborn scikit-learn
Python version used: 3.10+
Libraries:

pandas
numpy
matplotlib
seaborn
scikit-learn

No additional installations are needed.
🚀 How to Run

Clone the repositoryBashgit clone https://github.com/your-username/student-performance-prediction.git
cd student-performance-prediction
Download the dataset
Go to the Kaggle page
Download StudentsPerformance.csv
Place it in the project root directory

Start Jupyter NotebookBashjupyter notebookorBashjupyter lab
Open and run finalProject.ipynb
Execute all cells step by step
The notebook will automatically save cleaned data and display all visualizations and results


📈 Key Results
Conclusions:

Random Forest significantly outperforms the linear baseline.
The most important factors influencing math scores are:
Test preparation course completion
Parental education level
Lunch type (proxy for socioeconomic status)

There is still room for improvement (R² ≈ 0.20) – possible next steps: Gradient Boosting models (XGBoost, LightGBM), more feature engineering, or including reading/writing scores as predictors.

📊 Visualizations in the Notebook

Descriptive statistics table
Distribution histograms for scores
Boxplots by categorical features
Correlation heatmap
Actual vs Predicted scatter plot (comparison of both models)

🔮 Possible Improvements & Extensions

Try XGBoost, LightGBM, or CatBoost
Predict all three scores simultaneously (multi-output regression)
Use reading and writing scores as additional features
Perform more advanced feature engineering (e.g., average score, score differences)
Deploy the model as a simple web app (Streamlit/Flask)

🤝 Contributing
Contributions are welcome! Feel free to:

Open issues for bugs or suggestions
Submit pull requests with improvements
Add new models or visualizations

📄 License
This project is distributed under the MIT License. See LICENSE file for details.
The dataset is subject to Kaggle's original license and terms of use.

Submitted by: Amina Kabidesh | Nuray Bolat
Date: December 2025
Course: Machine Learning Semester Project























ModelRMSEMAER²Baseline (Linear Regression)~14.29~11.49~0.11Improved (Random Forest + GridSearchCV)~13.65~10.92~0.20
Conclusions:

Random Forest significantly outperforms the linear baseline.
The most important factors influencing math scores are:
Test preparation course completion
Parental education level
Lunch type (proxy for socioeconomic status)

There is still room for improvement (R² ≈ 0.20) – possible next steps: Gradient Boosting models (XGBoost, LightGBM), more feature engineering, or including reading/writing scores as predictors.

📊 Visualizations in the Notebook

Descriptive statistics table
Distribution histograms for scores
Boxplots by categorical features
Correlation heatmap
Actual vs Predicted scatter plot (comparison of both models)

🔮 Possible Improvements & Extensions

Try XGBoost, LightGBM, or CatBoost
Predict all three scores simultaneously (multi-output regression)
Use reading and writing scores as additional features
Perform more advanced feature engineering (e.g., average score, score differences)
Deploy the model as a simple web app (Streamlit/Flask)

🤝 Contributing
Contributions are welcome! Feel free to:

Open issues for bugs or suggestions
Submit pull requests with improvements
Add new models or visualizations

📄 License
This project is distributed under the MIT License. See LICENSE file for details.
The dataset is subject to Kaggle's original license and terms of use.

Author: [Your Name]
Date: December 2025
Course: Machine Learning Semester Project
