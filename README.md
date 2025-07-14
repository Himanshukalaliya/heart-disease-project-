# Heart Disease Risk Prediction Dashboard

## Overview
This project aims to predict the likelihood of heart disease using clinical data from the Cleveland Heart Disease dataset. It combines machine learning classification models with Power BI for insightful, interactive data visualization.

## Objectives
- Analyze medical indicators such as age, cholesterol, blood pressure, and chest pain type
- Predict risk of heart disease (binary classification: 0 = No disease, 1 = Disease)
- Build an interactive Power BI dashboard for stakeholders
- Identify key patterns and trends among high-risk patient segments

## Tech Stack
- **Python**: Data processing and machine learning
  - Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
- **Power BI**: Interactive data visualizations and reports
- **Jupyter Notebook** or **VS Code**
- **Dataset**: Cleveland Heart Disease dataset (UCI Repository)

## Machine Learning Workflow
1. **Data Cleaning**
   - Handle missing values
   - Convert categorical data to numeric (e.g., chest pain types, thalassemia)
   - Create derived features (e.g., age group, cholesterol level)
2. **Model Building**
   - Models used: Logistic Regression, Random Forest, and Support Vector Machine
   - Evaluate performance using accuracy, confusion matrix, and classification report
3. **Export Predictions**
   - Final CSV file includes input features and prediction column
   - Used as input in Power BI dashboard

## Power BI Dashboard Features
- Summary cards for total patients, disease count, and model accuracy
- Interactive charts: Disease by age, cholesterol, chest pain, thal
- Slicers for filtering by gender, fasting blood sugar, and age group
- Risk segmentation based on multiple features

## File Structure
```
heart_disease_prediction/
├── data/
│   └── heart.csv
├── models/
│   └── final_model.pkl
├── notebooks/
│   └── heart_disease_analysis.ipynb
├── powerbi/
│   └── dashboard.pbix
└── README.md
```

## Results Summary
- Model Accuracy: ~85%
- Key influencing features: `cp`, `thalach`, `ca`, `oldpeak`
- Observed higher risk in males aged 50–60 with elevated cholesterol and abnormal ECG

## How to Run the Project

**Python (Model Training)**  
1. Clone the repository  
2. Run `heart_disease_analysis.ipynb` to train and evaluate the model  
3. Export predictions to CSV

**Power BI**  
1. Open `dashboard.pbix`  
2. Connect to the updated CSV  
3. Refresh visuals to explore risk patterns
