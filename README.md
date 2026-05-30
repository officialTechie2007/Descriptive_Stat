# Descriptive Statistics with Python

## Overview

This repository contains a comprehensive implementation of fundamental Descriptive Statistics concepts using Python. The notebook explores statistical measures, probability distributions, data visualization techniques, outlier detection methods, and relationship analysis between variables.

The project is designed to provide both theoretical understanding and practical implementation of statistical concepts that serve as the foundation for Data Science, Machine Learning, and Data Analysis.

---

## Objectives

* Understand the structure and characteristics of datasets.
* Summarize data using statistical measures.
* Detect and analyze outliers.
* Visualize distributions and patterns.
* Explore probability distributions.
* Analyze relationships between variables.
* Build intuition for data preprocessing in Machine Learning.

---

## Recommended Prerequisites

To gain the most value from this notebook, readers should have basic familiarity with:

- Python Programming
- NumPy
- Pandas
- Basic Probability
- Elementary Algebra
- Data Visualization Concepts

No prior Machine Learning knowledge is required.


## Learning Outcomes

After completing this notebook, readers will be able to:

- Compute and interpret measures of central tendency
- Analyze data dispersion using variance and standard deviation
- Understand quartiles and the five-number summary
- Detect outliers using Z-Score and IQR methods
- Visualize distributions using histograms and KDE plots
- Interpret PDF and CDF curves
- Explore Normal, Log-Normal, and Pareto distributions
- Analyze relationships using covariance and correlation
- Apply descriptive statistics to real-world datasets such as Iris



## Why Descriptive Statistics Matters in Machine Learning?

Descriptive statistics forms the foundation of Exploratory Data Analysis (EDA). Before training machine learning models, data scientists use descriptive statistical techniques to:

- Understand data distributions
- Detect anomalies and outliers
- Identify skewness and variability
- Explore feature relationships
- Guide feature engineering decisions
- Improve model reliability

A strong understanding of descriptive statistics is essential for effective data preprocessing and machine learning workflows.

---

# Topics Covered

---

## 1. Measures of Central Tendency

Measures of central tendency describe the central or typical value of a dataset.

### Mean

The arithmetic average of observations.

[
\bar{x}=\frac{\sum_{i=1}^{n}x_i}{n}
]

Properties:

* Uses all observations.
* Sensitive to outliers.
* Most commonly used measure of center.

### Median

The middle value of an ordered dataset.

Properties:

* Robust against outliers.
* Suitable for skewed distributions.

### Mode

The most frequently occurring observation.

Properties:

* Can be used for both numerical and categorical data.
* A dataset may have multiple modes.

---

## 2. Measures of Dispersion

Dispersion measures quantify the spread of data around a central value.

### Range

[
Range = Maximum - Minimum
]

### Variance

Measures average squared deviation from the mean.

[
\sigma^2 = \frac{\sum (x_i-\mu)^2}{N}
]

### Standard Deviation

Square root of variance.

[
\sigma = \sqrt{\sigma^2}
]

Properties:

* Expressed in the same unit as the data.
* Indicates consistency or variability.

### Coefficient of Variation

[
CV=\frac{\sigma}{\mu}\times100
]

Used for comparing variability across datasets.

---

## 3. Five Number Summary

A concise summary describing distribution characteristics.

Components:

1. Minimum
2. First Quartile (Q1)
3. Median (Q2)
4. Third Quartile (Q3)
5. Maximum

Provides insights into spread, skewness, and outliers.

---

## 4. Box Plot Analysis

Box plots visualize distribution characteristics using quartiles.

Features:

* Median
* Interquartile Range (IQR)
* Potential outliers
* Data spread
* Skewness

### Interquartile Range

[
IQR = Q3 - Q1
]

Outlier Boundaries:

[
Lower = Q1 - 1.5(IQR)
]

[
Upper = Q3 + 1.5(IQR)
]

---

## 5. Outlier Detection

Outliers are observations significantly different from the majority of data.

### Z-Score Method

Measures distance from mean in standard deviation units.

[
Z=\frac{x-\mu}{\sigma}
]

Common Rule:

[
|Z| > 3
]

Observation is considered an outlier.

### IQR Method

Based on quartiles and resistant to extreme values.

Suitable for skewed datasets.

---

## 6. Histogram

A graphical representation of frequency distribution.

Applications:

* Understanding shape of data.
* Detecting skewness.
* Identifying multiple peaks.
* Detecting potential outliers.

---

## 7. Probability Density Function (PDF)

Describes the relative likelihood of a continuous random variable.

Properties:

[
P(a \leq X \leq b)
==================

\int_a^b f(x),dx
]

Area under the PDF equals 1.

---

## 8. Cumulative Distribution Function (CDF)

Represents cumulative probability up to a value.

[
F(x)=P(X\le x)
]

Properties:

* Monotonically increasing.
* Ranges from 0 to 1.

---

## 9. Kernel Density Estimation (KDE)

A non-parametric technique used to estimate probability density.

Advantages:

* Smooth alternative to histograms.
* Better visualization of distribution shape.
* Useful for identifying multimodal behavior.

---

## 10. Iris Dataset Analysis

The Iris dataset is one of the most widely used datasets in Data Science.

Features:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

Classes:

* Setosa
* Versicolor
* Virginica

Applications:

* Exploratory Data Analysis
* Classification
* Statistical Visualization

---

# Probability Distributions

---

## 11. Normal Distribution

A symmetric bell-shaped distribution.

[
X \sim N(\mu,\sigma^2)
]

Characteristics:

* Mean = Median = Mode
* Symmetric around the mean
* Foundation of many statistical methods

---

## 12. Log-Normal Distribution

A variable follows a log-normal distribution if its logarithm follows a normal distribution.

[
Y=\ln(X)
]

Applications:

* Income distributions
* Biological measurements
* Financial data

Characteristics:

* Positively skewed
* Non-negative values

---

## 13. Pareto Distribution

Models situations where a small percentage contributes to a large proportion of outcomes.

Commonly known as the 80-20 Principle.

Examples:

* Wealth distribution
* Business sales
* Website traffic

Characteristics:

* Heavy-tailed distribution
* Significant extreme events

## Distribution Visualizations

The notebook includes graphical representations of:

- Normal Distribution
- Log-Normal Distribution
- Pareto Distribution

These visualizations help understand:
- Symmetry
- Skewness
- Tail behavior
- Probability density characteristics

---

# Relationship Analysis

---

## 14. Covariance

Measures directional relationship between variables.

[
Cov(X,Y)
========

\frac{\sum (X_i-\bar X)(Y_i-\bar Y)}
{n-1}
]

Interpretation:

* Positive → variables increase together.
* Negative → inverse relationship.
* Near zero → weak linear relationship.

---

## 15. Pearson Correlation

Measures linear association.

[
r=
\frac{Cov(X,Y)}
{\sigma_X\sigma_Y}
]

Range:

[
-1 \le r \le 1
]

Interpretation:

* +1 : Perfect positive relationship
* 0 : No linear relationship
* -1 : Perfect negative relationship

---

## 16. Spearman Rank Correlation

Measures monotonic relationships using ranks.

Useful when:

* Data is not normally distributed.
* Relationship is non-linear.
* Outliers are present.

Range:

[
-1 \le \rho \le 1
]

---

# Libraries Used

* NumPy
* Pandas
* Matplotlib
* Seaborn
* SciPy
* Scikit-Learn

---

# Project Structure

```
Descriptive_Statistics/
│
├── Descriptive_Statistics.ipynb
├── requirements.txt
├── README.md
└── images/
```

---

# Future Enhancements

* Inferential Statistics
* Confidence Intervals
* Hypothesis Testing
* ANOVA
* Chi-Square Tests
* Probability Theory
* Feature Engineering

---

# Author

Akinchan Nayek

Exploring the foundations of Data Science, Machine Learning, and Statistical Analysis through practical Python implementations.
