# mimiciv-SAAKI
Predicting Mortality in Critically Ill Patients with Sepsis-Associated Acute Kidney Injury

# Objective: 
To find the most optimal machine learning model for the dataset in order to predict mortality in patients to provide care for high at-risk individuals earlier.

# Background:
SA-AKI → Sepsis-Associated Acute Kidney Injury: A condition where kidney function deteriorates as a result of sepsis.
Sepsis can lead to systemic inflammation, decreased blood flow to vital organs, and the release of harmful substances into the bloodstream.
Kidneys play a crucial role in filtering waste products and excess fluids from the blood. When compromised, it can lead to acute kidney injury. 25%-75% of people are affected by SA-AKI, depending on severity and type

# Dataset:
MIMIC-IV contains patient data from 2008 - 2019 including patient demographics, diagnoses, lab results, treatments, procedures, etc.
Tables Used in Our Study:
Patients - To get patients demographics details
Diagnosis - To get patients affected by sepsis and other comorbidities
ICU - Patients admitted in ICU
Chartevents - To get the vitals
Labevents - To get the laboratory results 

# Data Preprocessing:
Encode Categorical Variables
Handle Missing Values using miceforest algorithm
Outlier Removal using IQR 
Feature Scaling: Standard Scaler to normalise the data 

# Model Building:
Models built :
Logistic Regression					
SVM							
KNN
Decision Tree
Random Forest
XGBoost
Cat Boost
LightGBM
Gradient Boost
Ada Boost
Used GridSearch for tuning hyperparameters
Used the best estimators to train the model to get best AUC.

# Results:
LightGBM yielded an area under the receiver operating characteristics (AUROC) of 0.821.


