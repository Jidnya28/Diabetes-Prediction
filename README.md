# Diabetes-Prediction
This project aims to predict the likelihood of Type 2 Diabetes using diagnostic and demographic health indicators. Using the PIMA Indian Diabetes dataset, the study applies exploratory data analysis (EDA), data cleaning, feature scaling, and multiple machine learning models to build an effective classification system.
A major focus of the project is handling real-world data challenges, including:

Invalid zero values treated as missing data

Class imbalance between diabetic and non-diabetic patients

Model bias toward the majority class

To address these issues, the project evaluates Logistic Regression and Decision Tree models under:

Original data distribution

Oversampling

Undersampling

SMOTE (Synthetic Minority Oversampling Technique)

The final goal is to improve recall for diabetic patients, minimizing Type II errors, which are critical in healthcare prediction systems.

🗂️ Dataset

The dataset is sourced from the National Institute of Diabetes and Digestive and Kidney Diseases and consists exclusively of female patients aged 21 years and above of Pima Indian heritage.

📊 Dataset Structure

Rows: 768 patients

Columns: 9 (8 features + 1 target variable)

🎯 Target Variable

Outcome

0 → Non-diabetic

1 → Diabetic

🔢 Feature Description

Pregnancies – Number of times pregnant

Glucose – Plasma glucose concentration (2-hour oral glucose tolerance test)

BloodPressure – Diastolic blood pressure (mm Hg)

SkinThickness – Triceps skin fold thickness (mm)

Insulin – 2-hour serum insulin (mu U/ml)

BMI – Body Mass Index (kg/m²)

DiabetesPedigreeFunction – Genetic risk score based on family history

Age – Age of the patient (years)

🔍 Data Quality Observations

No explicit missing values

Several medical features contained zero values, which are biologically invalid

Zero values were treated as missing data (NaN) and imputed using:

Mean for normally distributed variables

Median for skewed variables

⚖️ Class Imbalance

Majority class: Non-diabetic (0)

Minority class: Diabetic (1)

This imbalance required specialized handling using:

Oversampling

Undersampling

SMOTE
