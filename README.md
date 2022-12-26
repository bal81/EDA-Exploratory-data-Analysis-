# EDA-Exploratory-data-Analysis-

![Exploratory data analysis for breast cancer prediction]/Users/baldervillagomez/Documents/UoM/mio/mio/jobs_App/2022/myrepo/Breast_Cancer/angiola-harry-nJv6xnlpNaA-unsplash.jpg

Data science is having a huge impact on the medical field, specifically in the area of cancer studies. In this project I will work with breast cancer data. This project focuses on data analysis using a simple step-by-step explanation.

# Table of Contents carry out in the Notebook
1. [Chapter 1 - Project Overview](#ch1)
1. [Chapter 2 - EDA Definition and Steps](#ch2)
1. [Chapter 3 - Step 1: Data Gathering](#ch3)
1. [Chapter 4 - Step 2: Head and describe](#ch4)
1. [Chapter 5 - Step 3: Target distribution](#ch5)
1. [Chapter 6 - Step 4: Features distribution](#ch6)
1. [Chapter 7 - Step 5: Correlation matrix](#ch7)
1. [Chapter 8 - Step 6:  Correlated features](#ch8)
1. [Chapter 9 - Step 7: Dimensionality reduction and scaling of features](#ch10)
1. [Chapter 10 - Step 9: Data Modelling](#ch10)
1. [Chapter 12 - Step 10: Conclusion and saving the model](#ch10)

<a id="ch1"></a>
# Project Overview

# **Project Summary from Kaggle:**

Features are computed from a digitized image of a breast mass. The cell nuclei in the image have certain characteristics. n the 3-dimensional space is that described in: [K. P. Bennett and O. L. Mangasarian: "Robust Linear Programming Discrimination of Two Linearly Inseparable Sets", Optimization Methods and Software 1, 1992, 23-34].

This database is also available through the UW CS ftp server:
- ftp ftp.cs.wisc.edu
- cd math-prog/cpo-dataset/machine-learn/WDBC/

[Also can be found on UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29)

# Attribute information:

- ID number
- Diagnosis ( [1]: M = Malignant(Cancerous) or [0]: B = Benign(Not Cancerous))

# Ten real-valued features are computed for each cell nucleus:

- radius (mean of distances from center to points on the perimeter)
- texture (standard deviation of gray-scale values)
- perimeter
- area
- smoothness (local variation in radius lengths)
- compactness (perimeter^2 / area - 1.0)
- concavity (severity of concave portions of the contour)
- concave points (number of concave portions of the contour)
- symmetry
- fractal dimension ("coastline approximation" - 1)

Each image was analyzed for 30 features. The mean, standard error, and largest value of these features were computed. For example, the field "Mean Radius" is in field 3, the field "Radius SE" is in field 13, and the field "Worst Radius" is in field 23.

* All feature values are recoded with four significant digits

* Missing attribute values: none

* Class distribution: 357 benign, 212 malignant

Let's take a look at the steps:  

<a id="ch2"></a>
# EDA Definition and Steps

![Exploratory data analysis steps](/images/breast_cancer/breast_cancer1.jpg)

Exploratory data analysis is a method used by data scientists to investigate and summarize the characteristics of data sets. This can often be done through data visualization methods. The data science tool helps determine how best to use data sources to get the answers we need. This makes it easier for data scientists to discover patterns, spot anomalies, test a hypothesis, or check assumptions.

EDA is a versatile data analysis tool that can help researchers and developers better understand the relationships between data set variables. The EDA techniques can help you determine if the statistical techniques you are considering are appropriate for the data you are working with.Originally developed by American mathematician John Tukey, these techniques are still widely used today in the data discovery process.

The process of data analysis involves organizing and summarizing the raw data, discovering important features and patterns in the data, and interpreting the findings.

Some outcomes of EDA:

- Extracting averages, mean, minimum, and maximum values can help us better understand variables.
- We can use the data to identify obvious potenital errors, outliers, and missing values.
- Identify patterns in data by visualizing it in graphs. For example, box plots, scatter plots, and histograms can help us see patterns in the data.

In this summary, I will focus on the steps of EDA. I will explain what each step is and what it involves.:

- Data head and describe data (viewing data and its statistical information)
- Target distribution (this is the distribution of malignant and benign data)
- Features distribution (this is the distribution between the features)
- Correlation matrix (this is a table that displays the correlation coefficients between different variables)
- Positive correlated features
- Uncorrelated features
- Negative correlated features 
