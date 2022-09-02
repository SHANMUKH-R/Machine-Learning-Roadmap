# Machine Learning Collection

This is a step by step process where you explore what you wanna learn, know where to lie and dive deeper. I believe, there is nothing such as perfection at learning 
a topic but teaching does the job. I will try to make the code as clear as possible. This repository is contribution friendly, so if you feel you want to add something 
then I'd happily merge a PR.

## DATA PREPROCESSING
>Coversion of raw data into a clean dataset and making it suitable for a machine learning model. 

**Myth** - Data is collected, organised and fed into model.

**Fact** - **FORBES**: Data scientists spend around 80% of their time on preparing and managing data. Data preprocessing is the method of analyzing, filtering, transforming and encoding data so that a machine learning algorithm can understand and work with the processed output.

![data scientists pie chart](https://user-images.githubusercontent.com/71865643/187874766-d8560679-42af-4c11-9a73-8c7c33e8523b.jpg)

## Why Data Preprocessing

So why exactly? There is a popular saying that goes as 
> **"if garbage goes in, garbage comes out"**. 

>In real world senarios, there’s always noise and missing values. This happens due to manual errors, unexpected events, technical issues, or a variety of other obstacles.

## Purpose:

**Identify Missing Data** 

> Missing data can disrupt data patterns. This is common in real world senarios and it's an important step to handle missing data instead of removing the colums or rows because of a few missing cells.

**Identify outliers or anomalous data** 

>  An outliner is a datapoint that lies extrmely high or extremely low from rest of the neighboring co-existing values. Simply, an datapoint that standsout a lot. An anamalous datapoint is similar to outliners and can be defined in a better way as rare item that differ significantly from standard behaviors or patterns.

**Remove Inconsistencies** 

>  Incorrect spellings, incorrectly populated columns and rows (eg.: salary populated in gender column), duplicated data are examples of inconsitencies.

## Data Preprocessing - Step 1 - Importing Libraries

> **Pandas** - Open source python package most widely used for data manupulation and analysis

> **Numpy** - Numpy is a python package for handling multi-dimensional array and matrix with the help of large collection of high-level mathematical functions.

> **Matplotlib** - A comprehensive library for creating static, animated and interactive visualizations in python. Supports various types of graphical representations like Bar Graphs, Histograms, Line Graph, Scatter Plot, Stem Plots, etc.


<p align="center">
<img width="520" alt="Importing libraries" src="https://user-images.githubusercontent.com/71865643/187871198-eb8c90bf-8cd8-42df-9a91-0d92d3db8e10.png"></p>


## Data Preprocessing - Step 2 - Handling Missing Data

**How**
> SimpleImputer is a scikit-learn class which is helpful in handling the missing data in the dataset. Replace missing values using a descriptive statistic (e.g. mean, median, or most frequent) along each column, or using a constant value.

<p align='center'><img width="520" alt="Handling Missing Datas" src="https://user-images.githubusercontent.com/71865643/187905086-09ac03a1-ea51-4538-857a-3f7ffa082150.png"></p>

**SimpleImputer() Parameters:**

> **missing_values** - For pandas dataframes with nullable integer dtypes with missing values, missing_values can be set to either np.nan or pd.NA.
> **Strategy** - This indicates the imputation strategy
>               : Takes in String as input, default = 'mean' 
>               : If “mean”, then replace missing values using the mean along each column. Can only be used with numeric data.
>               : If “median”, then replace missing values using the median along each column. Can only be used with numeric data.
>               : If “most_frequent”, then replace missing using the most frequent value along each column. Can be used with strings or numeric data. If there is more than one such value, only the smallest is returned.
>               :If “constant”, then replace missing values with fill_value. Can be used with strings or numeric data. 


