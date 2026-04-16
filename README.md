# 🧠 Breast Cancer Survival Analysis Using Python

A Python-based data analysis project focused on exploring breast cancer survival patterns using real-world data from the SEER dataset. This project applies data cleaning, exploratory data analysis, feature evaluation, statistical techniques, and survival analysis to identify key factors influencing survival outcomes.

---

## 📌 Project Overview

This project performs end-to-end analysis on breast cancer survival data to understand how demographic and clinical variables affect patient outcomes. The analysis combines exploratory data analysis, feature selection, statistical comparison, and Kaplan–Meier survival curves to extract meaningful and interpretable insights.

The project also investigates **ethnicity-based survival disparities** across Black, White, and Other patient groups, and examines whether these differences remain after controlling for clinical severity factors such as tumor size and AJCC stage.

---

## 🎯 Objectives

- Clean and preprocess raw breast cancer survival data  
- Explore survival trends using visualizations  
- Identify important clinical and demographic features  
- Analyze relationships between variables and survival outcome  
- Apply statistical techniques to extract insights  
- Compare survival across ethnic groups and disease stages  
- Present results in a clear and interpretable manner  

---

## 🗂️ Dataset Information

**Dataset Source:** SEER Breast Cancer Dataset  
**Source Type:** Public cancer registry data from the National Cancer Institute (NCI)  
**Population:** Female breast cancer patients in the United States  
**Coverage:** Approximately 28% of the U.S. population  

### Key Variables

- **Demographics:** Age, Race/Ethnicity, Marital Status  
- **Clinical:** T Stage, N Stage, AJCC 6th Stage, Grade, A Stage  
- **Tumor:** Tumor Size (mm), Estrogen Status, Progesterone Status  
- **Outcome:** Survival Months, Status (Alive/Dead)  

---

## 🛠️ Tools & Technologies

- Python 3  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Lifelines  
- Openpyxl  
- Jupyter Notebook  

---

## 🔄 Workflow

1. Data Loading & Inspection  
2. Data Cleaning & Preprocessing  
3. Exploratory Data Analysis (EDA)  
4. Correlation Analysis  
5. Mutual Information Analysis  
6. Stability-based Feature Selection  
7. Survival Comparison & Visualization  
8. Ethnicity-Based Survival Analysis  
9. Kaplan–Meier Curve Analysis  
10. Statistical Interpretation of Results  

---

## 📊 Analysis Pipeline

### 1. Data Cleaning
- Loaded the dataset
- Removed irrelevant columns
- Handled missing values
- Dropped duplicate rows
- Encoded categorical variables

### 2. Statistical Analysis
- Performed descriptive statistics
- Compared group-wise means for Alive vs Dead cases
- Studied standard deviation and data spread

### 3. EDA & Visualization
- Survival status distribution
- Tumor size boxplot
- Correlation heatmap

### 4. Mutual Information
- Measured predictive power of each feature on survival outcome
- Captured non-linear relationships between variables

### 5. Stability Selection
- Used bootstrapped mutual information over 100 iterations
- Identified consistently important features

### 6. Ethnicity Analysis
- Calculated survival percentage for each ethnic group
- Performed baseline unadjusted comparison

### 7. Stage-Based Analysis
- Studied AJCC 6th Stage distribution across ethnic groups
- Measured stage-wise survival and death rates

### 8. Controlled Ethnicity Comparison
- Compared survival within the same stage and tumor size groups
- Evaluated whether disparities persist after adjustment

### 9. Odds of Death
- Calculated odds of death for each ethnic group by AJCC stage and tumor size group

### 10. Kaplan–Meier Curves
- Generated survival curves by ethnicity
- Applied log-rank test for statistical significance

---

## 📈 Key Findings

- Black patients had the lowest survival rate at **74.9%**, compared to **85.1%** for White patients and **89.7%** for Other patients.
- The survival gap between Black and White patients was **14.8%**.
- For **Stage IIIC**, the odds of death were:
  - Black: **0.91**
  - White: **0.63**
  - Other: **0.30**
- In the **84–112 mm tumor size group**, Black patients had odds of death of **1.33**, meaning more deaths than survivors in that group.
- The **log-rank test** showed a statistically significant difference in survival curves:
  - **Chi-square = 30.98**
  - **p-value = 1.9 × 10⁻⁷**
- Survival disparities persisted even after controlling for AJCC stage and tumor size, suggesting that additional factors such as healthcare access, socioeconomic conditions, and treatment differences may contribute to the observed gap.

---
