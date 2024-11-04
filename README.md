# Predicting Diabetes Risk for SDG 3: Good Health and Well-being

## Project Overview
This project is part of Assignment 1 for SDG 3: Good Health and Well-being, which aims to ensure healthy lives and promote well-being for all at all ages. Using the **PIMA Indian Diabetes Dataset**, we developed a machine learning model to predict the likelihood of diabetes in individuals based on their medical and demographic data. This model can assist in early detection and intervention, contributing to improved health outcomes aligned with UN Sustainable Development Goal 3.

## Dataset
The dataset used is the **PIMA Indian Diabetes Dataset**, which includes health-related information for predicting diabetes. The features include:
- `Pregnancies`: Number of times pregnant
- `Glucose`: Plasma glucose concentration
- `BloodPressure`: Diastolic blood pressure
- `SkinThickness`: Triceps skin fold thickness
- `Insulin`: 2-hour serum insulin
- `BMI`: Body mass index (weight in kg/(height in m)^2)
- `DiabetesPedigreeFunction`: Family history of diabetes
- `Age`: Age in years
- `Outcome`: Diabetes indicator (1 = diabetic, 0 = non-diabetic)

## Project Workflow

### 1. Data Preprocessing
   - Replaced missing values with **median** for columns with potential outliers (e.g., `Insulin`, `BMI`) and **mean** for more balanced columns (e.g., `Glucose`).
   - Scaled the features using `StandardScaler` to improve model performance.

### 2. Model Selection and Evaluation
   - Tried multiple ML models:
     - **Logistic Regression**
     - **Decision Tree Classifier**
     - **Random Forest Classifier**
   - Performed **K-Fold Cross Validation** to validate each model, using the following metrics:
     - **Accuracy**
     - **Precision**
     - **Recall**
     - **F1-Score**
     - **Kappa Statistics**

### 3. Result Analysis
   - Analyzed each model's performance based on the cross-validation results.
   - Compared metrics across models to identify the best-performing algorithm for predicting diabetes risk.

### 4. Outputs
   - Results for Logistic Regression:
      - Accuracy: 0.7708598590951532
      - Precision: 0.7244260462898302
      - Recall: 0.5597484276729561
      - F1-Score: 0.630602221319156
      - Kappa: 0.4684104673391629
     
  - Results for Decision Tree:
     - Accuracy: 0.7162549868432222
     - Precision: 0.6001970302242041
     - Recall: 0.5860237596086653
     - F1-Score: 0.5912724932465709
     - Kappa: 0.3744411063457848
    
 - Results for Random Forest:
     - Accuracy: 0.7578728461081402
     - Precision: 0.6745620181791172
     - Recall: 0.6009783368273934
     - ...
     - Kappa: 0.45409839442244626
