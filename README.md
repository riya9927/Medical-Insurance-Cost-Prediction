# Medical Insurance Cost Prediction

## Overview
This project involves analyzing a medical insurance dataset and building a predictive model to estimate a person's insurance cost based on their demographic and health-related attributes. The dataset includes features such as age, BMI, smoking status, and region, which help determine the medical charges incurred by an individual.

---

## Dataset Details

**File Name:** `insurance_1741527527948.csv`

### Columns:
- **Age**: Age of the insured individual  
- **Sex**: Gender (`male` / `female`)  
- **BMI**: Body Mass Index, an indicator of body fat based on height and weight  
- **Children**: Number of children covered by the insurance policy  
- **Smoker**: Whether the person smokes (`yes` / `no`)  
- **Region**: Geographic region (`northeast`, `northwest`, `southeast`, `southwest`)  
- **Charges**: Total medical insurance cost incurred (Target variable)  

---

## Objective
To develop a **regression model** that predicts medical insurance charges based on demographic and health-related features.

---

## Implementation Steps

### 1. Data Preprocessing
- Load the dataset using `pandas`
- Check for missing values and handle any data inconsistencies
- Perform descriptive statistics

### 2. Exploratory Data Analysis (EDA)
- **Univariate Analysis**: Distribution plots for age, BMI, and charges
- **Bivariate Analysis**: Scatter plots for BMI vs. Charges, Age vs. Charges
- **Correlation Analysis**: Heatmaps to visualize relationships between features
- **Categorical Analysis**: Box plots for `smoker`, `sex`, and `region`

### 3. Feature Engineering
- Selecting relevant features: `Age`, `BMI`, `Children`, `Smoker`, `Region`
- One-hot encoding categorical variables (`Sex` and `Region`)
- Splitting dataset into **training (70%)** and **testing (30%)** sets

### 4. Model Training
- Train a **Linear Regression Model** using `scikit-learn`
- Fit the model on the training dataset
- Predict insurance charges on the test dataset

### 5. Model Evaluation
- Compute **R² score** to assess model accuracy
- Scatter plot to compare **actual vs. predicted** values

### 6. Prediction on New Data
- Provide a sample input for a new patient
- Predict their estimated insurance cost

---

## Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**

---

## Results
- The **Linear Regression model** achieved an **R² score of 0.85**, indicating strong predictive performance.
- **Smoking status** was the most significant factor affecting insurance costs, followed by **BMI and age**.

