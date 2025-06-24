# Exploratory Data Analysis (EDA) Summary – Titanic Dataset
## Objective
The goal of this EDA was to understand the Titanic dataset by exploring the structure, detecting patterns, identifying missing values or anomalies, and gaining insights into what factors influenced passenger survival. This forms the foundation for further preprocessing and modeling.
## What We Did
Loaded the Dataset

We imported the Titanic dataset using Pandas and previewed it using .head() and .info() to get a sense of the data types, columns, and missing values.

### Generated Summary Statistics

Used .describe() to compute basic statistics like mean, median, standard deviation, and ranges for numerical features like Age and Fare.

Checked categorical data distributions using value_counts() and .describe(include='object').

### Visualized Distributions

Created histograms and boxplots for numeric features to observe distribution, central tendency, and outliers.

Plotted the distribution of Age, Fare, etc., to understand variability across passengers.

### Explored Feature Relationships

Used Seaborn’s pairplot and heatmap to examine correlation and relationships between features such as Age, Pclass, Fare, and Survived.

Investigated categorical features like Sex and Pclass using countplots segmented by Survived.

### Handled Missing Values (Assessment)

Identified missing values using .isnull().sum() and visualized them using the missingno library.

Found that columns like Cabin had substantial missing data and noted them for imputation or removal.

### Advanced Visualizations 

Leveraged Plotly for interactive visuals to better understand how variables like Age and Fare affected survival.

## Why We Did It
Understand Data Composition: To assess data quality and content before applying any machine learning model.

Find Patterns & Trends: Identify important features that affect survival—like class, sex, and age.

Spot Anomalies & Outliers: Use boxplots to detect unusual values that may skew analysis.

Examine Relationships: Reveal how features correlate with each other and with the target variable Survived.

Guide Preprocessing: Missing value checks help decide what needs to be cleaned, filled, or removed.

## Key Insights
Sex: Females had significantly higher survival rates than males.

Pclass: Passengers in 1st class were more likely to survive.

Fare: Higher fare correlated with better survival odds.

Age: Younger children had better survival rates; outliers in fare and age were also observed.

Missing Data: ‘Cabin’ and some Age values were missing, signaling need for imputation or removal.

---
## By Harsimran Singh