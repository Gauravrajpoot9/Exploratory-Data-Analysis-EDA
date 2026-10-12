# Task-2-Exploratory-Data-Analysis-EDA---Comprehensive-Guide
The primary objective of this project is to extract meaningful insights from raw data through data cleaning, preprocessing, visualization, and statistical analysis. EDA helps identify patterns, trends, anomalies, and relationships within the dataset before applying machine learning models.
# Titanic Dataset - Exploratory Data Analysis (EDA)

## Project Overview

This project performs Exploratory Data Analysis (EDA) on the Titanic dataset using Python.

The main goal of this project is to:

* understand the dataset,
* clean the data,
* analyze patterns,
* create visualizations,
* detect outliers,
* study relationships between variables,
* and generate useful insights.

This project is beginner-friendly and helps in learning basic data analysis techniques.

---

# Dataset Information

The dataset contains information about Titanic passengers.

## Columns Used

| Column Name             | Description                                 |
| ----------------------- | ------------------------------------------- |
| Survived                | Passenger survived or not (0 = No, 1 = Yes) |
| Pclass                  | Passenger class (1st, 2nd, 3rd)             |
| Name                    | Passenger name                              |
| Sex                     | Gender                                      |
| Age                     | Passenger age                               |
| Siblings/Spouses Aboard | Number of siblings/spouses aboard           |
| Parents/Children Aboard | Number of parents/children aboard           |
| Fare                    | Ticket fare                                 |

---

# Technologies Used

* Python
* Pandas
* NumPy
* Seaborn
* Matplotlib
* SciPy

---

# Libraries Installation

Install required libraries using:

```bash
pip install pandas numpy seaborn matplotlib scipy
```

---

# Steps Performed in the Project

## 1. Data Loading

* Loaded dataset using Pandas.
* Checked rows and columns.

```python
df = pd.read_csv("titanic.csv")
```

---

## 2. Dataset Inspection

Performed:

* shape checking
* data type checking
* missing value detection
* duplicate row detection

Functions used:

```python
df.shape
df.dtypes
df.isnull().sum()
df.duplicated().sum()
```

---

## 3. Data Cleaning

* Removed duplicate rows.
* Checked for missing values.

```python
df.drop_duplicates()
```

---

## 4. Feature Engineering

Created new columns:

* FamilySize
* IsAlone

Purpose:

* understand family impact on survival.

---

## 5. Distribution Analysis

Visualized:

* age distribution
* fare distribution
* survival distribution
* gender distribution

Charts used:

* Histogram
* Countplot

---

## 6. Survival Analysis

Compared survival using:

* gender
* passenger class
* family size

Key observation:

* females survived more than males.
* first-class passengers had better survival rates.

---

## 7. Correlation Analysis

Used:

* heatmap
* correlation matrix
* crosstab analysis

Purpose:

* understand relationships between variables.

---

## 8. Outlier Detection

Detected fare outliers using:

* boxplot
* z-score method

Purpose:

* identify unusually high ticket fares.

---

## 9. Advanced Visualizations

Used:

* FacetGrid
* Pairplot
* Boxplot
* Heatmap

Purpose:

* multivariable analysis
* pattern detection

---

# Statistical Analysis

Performed:

* Skewness
* Kurtosis
* Pearson Correlation
* Spearman Correlation

Purpose:

* understand distribution and relationships.

---

# Hypotheses Tested

## H1: Higher-class passengers survived more

Result: Confirmed ✅

## H2: Females survived more than males

Result: Confirmed ✅

## H3: Higher fare increased survival chances

Result: Confirmed ✅

---

# Key Insights

* Women had higher survival rates.
* First-class passengers survived more.
* Higher ticket fare passengers had better survival chances.
* Most passengers were between 20–40 years old.
* Family size affected survival probability.

---

# Project Outcome

This project helped in learning:

* data cleaning
* exploratory data analysis
* data visualization
* correlation analysis
* outlier detection
* feature engineering
* statistical analysis

---

# Conclusion

The Titanic dataset provides useful insights into passenger survival patterns.

Important factors affecting survival:

* gender
* passenger class
* fare
* family size

This project demonstrates how EDA helps convert raw data into meaningful insights.

