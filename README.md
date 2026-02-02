# Insurance Data Analysis

This notebook (`insurance.ipynb`) performs an exploratory data analysis (EDA) on an insurance dataset to understand the distribution of variables and their relationship with insurance charges. The analysis focuses on identifying patterns, outliers, and correlations that influence medical insurance costs.

---

## Dataset Overview

The dataset contains information about individuals and their insurance charges with the following features:

- age: Age of the individual
- sex: Gender (male/female)
- bmi: Body Mass Index
- children: Number of dependents
- smoker: Smoking status (yes/no)
- charges: Medical insurance charges

---

## Objectives

- Analyze the distribution of numerical features
- Understand categorical feature frequencies
- Identify outliers in the data
- Examine relationships between variables
- Study correlations with insurance charges

---

## Exploratory Data Analysis

### Numerical Feature Analysis
- Histograms with KDE plots were used for:
  - age
  - bmi
  - children
  - charges
- Observed skewness and spread in insurance charges
- BMI follows an approximately normal distribution
- Charges show a right-skewed distribution with high-value outliers

### Categorical Feature Analysis
- Count plots were generated for:
  - sex
  - smoker
  - children
- Majority of individuals are non-smokers
- Gender distribution is nearly balanced
- Most individuals have zero or one dependent

---

## Outlier Detection

- Boxplots were used for numerical features
- Significant outliers observed in:
  - bmi
  - charges
- High insurance charges are concentrated among a small subset of individuals

---

## Correlation Analysis

- A heatmap of numerical features was generated
- Key observations:
  - Charges have moderate correlation with age
  - Charges show noticeable correlation with bmi
  - Number of children has very weak correlation with charges
  - Age and BMI are weakly correlated with each other

---

## Tools and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Key Insights

- Smoking status (observed indirectly) plays a major role in high insurance charges
- Older individuals tend to incur higher medical costs
- BMI contributes to insurance charges but with moderate impact
- Extreme insurance costs are driven by a small number of outliers

---

## How to Run the Notebook

1. Clone the repository
2. Install required libraries
3. Open the notebook using Jupyter

```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook insurance.ipynb
