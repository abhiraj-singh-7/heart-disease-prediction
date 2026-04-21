# Heart Disease Prediction Using Machine Learning

## Overview
This project presents an end-to-end machine learning workflow for predicting heart disease using structured clinical patient data. The notebook covers data loading, data inspection, duplicate checking, exploratory data analysis, preprocessing, model training, and comparative evaluation across multiple classification algorithms.

## Objective
The goal of this project is to predict whether a patient is likely to have heart disease based on medical attributes such as age, chest pain type, cholesterol level, resting blood pressure, maximum heart rate, and other clinical indicators.

## Dataset Source
The dataset used in this project was obtained from Kaggle:

[Heart Disease Dataset on Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

According to the dataset description, the data traces back to 1988 and is based on four databases: Cleveland, Hungary, Switzerland, and Long Beach V. While the original source contains 76 attributes, this project uses the commonly shared 14-feature version for heart disease prediction.

## Features Used
The dataset contains the following columns:

- `age` — age of the patient
- `sex` — gender of the patient
- `cp` — chest pain type
- `trestbps` — resting blood pressure
- `chol` — serum cholesterol in mg/dl
- `fbs` — fasting blood sugar > 120 mg/dl
- `restecg` — resting electrocardiographic results
- `thalach` — maximum heart rate achieved
- `exang` — exercise induced angina
- `oldpeak` — ST depression induced by exercise relative to rest
- `slope` — slope of the peak exercise ST segment
- `ca` — number of major vessels colored by fluoroscopy
- `thal` — thalassemia category
- `target` — heart disease diagnosis (1 = disease, 0 = no disease)

## Project Workflow
This notebook follows a complete machine learning pipeline:

1. Load and inspect the dataset  
2. Examine data types, missing values, summary statistics, and duplicates  
3. Perform exploratory data analysis using visualizations  
4. Remove duplicate rows to improve data quality  
5. Split the data into training and testing sets  
6. Apply feature scaling where appropriate  
7. Train and evaluate multiple models:
   - Logistic Regression
   - K-Nearest Neighbors
   - Random Forest
8. Compare model performance using:
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - Confusion matrices

## Data Cleaning
During the inspection stage, a large number of duplicate rows were identified in the downloaded dataset version. To ensure a more reliable evaluation, duplicate entries were removed before model training and testing.

## Models Implemented
The following machine learning models were trained and compared:

- **Logistic Regression**
- **K-Nearest Neighbors**
- **Random Forest**

## Results
Among the tested models, **Logistic Regression** achieved the strongest overall performance on the cleaned dataset.

### Best Model Performance
- **Model:** Logistic Regression
- **Accuracy:** 80.3%
- **Precision:** 80.0%
- **Recall:** 84.9%
- **F1-Score:** 82.4%

These results show that a simpler linear model performed best on this cleaned version of the dataset, outperforming both KNN and Random Forest in the final comparison.

## Tools and Libraries
This project was built using:

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Repository Contents
- `heart_disease_prediction.ipynb` — main notebook containing the full analysis and modeling workflow
- `heart.csv` — dataset used in the project
- `README.md` — project documentation

## Key Takeaways
- Proper data inspection is essential before model training
- Duplicate removal can meaningfully affect evaluation quality
- Exploratory data analysis helps reveal distributions, imbalance patterns, and outliers
- Simpler models can outperform more complex ones when the data is cleaned and prepared carefully

## Future Improvements
Possible next steps for this project include:

- Hyperparameter tuning
- Cross-validation for more robust evaluation
- ROC curve and AUC analysis
- Additional classification models
- Deployment as a simple web application using Streamlit or Flask

## Author
**Abhiraj Singh**
