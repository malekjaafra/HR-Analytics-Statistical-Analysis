# HR Analytics — Statistical Analysis of Employee Attrition

**Authors:** Malek Jaafra & May Zariat
**Program:** 2nd Year Big Data & Data Analytics
**Language:** R

---

## Project Overview

This project presents a complete statistical analysis of the **IBM HR Analytics Employee Attrition & Performance** dataset.

The objective is to identify the key factors influencing employee turnover and explore relationships between demographic, professional, and financial variables using statistical methods.

---

## Dataset

* **Source:** Kaggle — IBM HR Analytics Employee Attrition & Performance Dataset
* **Size:** 1,470 employees × 35 variables
* **Target Variable:** Attrition (Yes/No)

---

## Project Workflow

### 1. Data Preprocessing

* No missing values detected
* Data cleaning and structure verification

### 2. Univariate Analysis

* Age distribution (mean: 36.9 years)
* Monthly income distribution
* Gender breakdown (60% Male / 40% Female)
* Attrition rate: 16.1%

### 3. Bivariate Analysis — Quantitative Variables

* Correlation matrix
* Linear regression: YearsAtCompany ~ MonthlyIncome (R² = 0.264)
* Confidence interval of monthly income: [6262 ; 6744]
* Kernel Density Estimation (KDE): Age × MonthlyIncome

### 4. Bivariate Analysis — Qualitative Variables

* Attrition vs Department (χ² p = 0.0045, significant)
* Attrition vs Gender (p = 0.29, not significant)
* Attrition vs BusinessTravel (p = 5.6e-06, significant)
* Correspondence Analysis (CA) on JobRole

### 5. Mixed Analysis

* Boxplot: MonthlyIncome ~ Department (ANOVA p = 0.041)
* Boxplot: Age ~ Attrition (ANOVA p < 0.001)

### 6. Multivariate Analysis

* Principal Component Analysis (PCA)

  * Dimension 1: 54.6%
  * Dimension 2: 20.0%
* Factor Analysis of Mixed Data (FAMD)

  * Cumulative variance: 34.4%

---

## Key Findings

| Factor          | Finding                                                                 |
| --------------- | ----------------------------------------------------------------------- |
| Business Travel | Employees travelling frequently show the highest attrition rate (24.9%) |
| Job Role        | Sales Representatives have the highest attrition rate (39.8%)           |
| Age             | Employees who leave are approximately 4 years younger on average        |
| Correlation     | TotalWorkingYears × MonthlyIncome (r = 0.77)                            |

---

## Technologies Used

* R
* RStudio
* R Markdown
* ggplot2
* FactoMineR
* factoextra
* corrplot
* MASS

---

## Project Structure

```text
HR-Analytics-Statistical-Analysis/
├── Projet_HR_Analytics.pdf
├── Projet_HR_Analytics.Rmd
├── dataset/
│   └── WA_Fn-UseC_-HR-Employee-Attrition.csv
└── README.md
```

---

## Authors

* Malek Jaafra
* May Zariat
