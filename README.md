# Titanic Survival Prediction 🚢

## Overview
This project predicts passenger survival on the Titanic using machine learning.  
It demonstrates **data cleaning, feature engineering, model training, model explainability, and interactive prediction**.

## Dataset
- [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)
- Features: Passenger class, sex, age, family size, fare, embarkation port, etc.
- Target: `Survived` (0 = No, 1 = Yes)

## Workflow
1. Exploratory Data Analysis (EDA)  
2. Feature Engineering  
   - Extract titles from names  
   - Create family size and IsAlone features  
   - Encode categorical variables  
3. Model Training  
   - Logistic Regression  
   - Random Forest  
   - XGBoost  
4. Evaluation  
   - Precision, Recall, F1 Score  
   - ROC-AUC  
5. Explainability (NEW)  
   - SHAP values to explain survival predictions  
6. Interactive Streamlit App (NEW)  
   - Users can enter age, class, sex → see survival prediction in real-time  

## Results
- Random Forest: **~82% accuracy**, ROC-AUC ~0.86  
- SHAP plots show importance of **Sex, Class, Age**  

## Usage
```bash
pip install -r requirements.txt
python titanic_train.py
