# Titanic Dataset – Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)
![Libraries](https://img.shields.io/badge/Libraries-Pandas%2C%20NumPy%2C%20Matplotlib%2C%20Seaborn-orange.svg)
![Jupyter](https://img.shields.io/badge/Environment-Jupyter%20Notebook-yellow.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

---

## 📖 Overview

This project performs **Exploratory Data Analysis (EDA)** on the classic **Titanic dataset** from Kaggle’s *Machine Learning from Disaster* competition.  
The goal is to explore patterns and trends that influenced passenger survival — such as **gender, class, age, fare, and embarkation port** — using Python’s data analytics and visualization libraries.

By conducting EDA, we aim to transform raw data into actionable insights that reveal *who survived and why*.

---

## 🎯 Objectives

- Understand dataset structure and data types  
- Handle missing values and inconsistent entries  
- Analyze feature distributions and detect outliers  
- Visualize relationships that affect survival  
- Identify the strongest predictors for survival outcomes  

---

## Tech Stack

| Category | Tools Used |
|-----------|-------------|
| **Language** | Python 3.9+ |
| **Libraries** | Pandas, NumPy, Matplotlib, Seaborn |
| **Environment** | VS Code + Jupyter Notebook |
| **Dataset Source** | [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data) |

---

---

## ⚙️ Data Preparation Steps

1. **Data Loading:** Imported `train.csv` using Pandas.  
2. **Data Cleaning:**
   - Filled missing `Age` with the **median** value.  
   - Filled missing `Embarked` with the **mode**.  
   - Dropped `Cabin` due to excessive missing values.  
3. **Data Type Fixes:** Converted numeric and categorical fields to proper datatypes.  
4. **Validation:** Checked that no missing data remained after cleaning.  

---

## 📊 EDA Process

### **1. Univariate Analysis**
Explored individual features:
- **Age:** Mostly 20–40 years; right-skewed.  
- **Fare:** Highly skewed; majority of fares under 100.  
- **Sex:** More male passengers than female.  
- **Class:** Majority traveled in 3rd class.  
- **Embarked:** Most passengers boarded from Southampton.

### **2. Bivariate Analysis**
Explored relationships between features and survival:
- **Gender:** Females had significantly higher survival rates.  
- **Class:** 1st class passengers had higher survival chances.  
- **Fare:** Higher fare correlated with better survival.  
- **Age:** Children and younger passengers survived more often.  
- **Embarked:** Passengers from Cherbourg (C) survived more frequently.

### **3. Multivariate Analysis**
Used correlation matrices and pairplots to visualize numeric relationships.
- `Fare` showed a positive correlation with `Survived`.  
- `Pclass` showed a negative correlation (lower class → lower survival).  
- Weak correlations between `SibSp`, `Parch`, and survival individually, but potentially useful when combined.

---

## 🔍 Key Insights

| Factor | Observation | Insight |
|:--------|:-------------|:---------|
| **Gender** | Women survived much more than men | “Women and children first” policy visible |
| **Class** | 1st class had the highest survival rate | Wealth & cabin proximity to lifeboats mattered |
| **Fare** | Higher fare = better survival | Fare correlates with passenger class |
| **Age** | Younger passengers survived more | Children were prioritized |
| **Embarked** | Port C > Port S > Port Q | Possible class differences by embarkation |

---

## 📈 Visual Highlights

The notebook includes clear, labeled plots for storytelling:
- Age and Fare distribution histograms  
- Countplots for gender, class, and embarkation  
- Boxplots comparing survival vs age and fare  
- Correlation heatmap of numeric features  
- Pairplot of major numeric relationships  

Each visual is followed by written observations to build a coherent data story.

---

## 💾 Output Files

| File | Description |
|------|--------------|
| `Titanic_EDA.ipynb` | Main notebook with all analysis & plots |
| `train_cleaned.csv` | Cleaned dataset (no missing values) |
| `Titanic_EDA_Report.pdf` | Exported PDF report with visuals and insights |

---

## What I Learned

- How to handle missing data using **median and mode imputation**  
- How to detect and interpret **skewed distributions**  
- How to find relationships through **countplots, boxplots, and heatmaps**  
- How to summarize insights from raw visual data  
- How to create a clean, documented EDA notebook ready for presentation  

---

## 🚀 How to Run This Project

1. **Clone this repository:**
   ```bash
   git clone https://github.com/<your-username>/Titanic_EDA_Project.git

