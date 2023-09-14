# EDA_Exploratory.Data.Analysis

Exploratory Data Analysis (EDA) is an approach to analyzing data sets to summarize their main characteristics, often with visual methods. Here are the steps involved in EDA:

1. Data Collection: This is the first step where you gather the data from various sources.

2. Data Cleaning: This step involves handling missing data, removing duplicates and outliers.

3. Data Wrangling or Data Munging: In this process, the raw data is transformed into another format to make it more suitable for analysis.

4. Data Analysis: In this step, various statistical techniques are used to analyze the data.

5. Data Visualization: This involves presenting your data in a visual format like graphs, charts etc., to understand the patterns, trends and insights in the data.

- Importing required libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

- Load the dataset
df = pd.read_csv('data.csv')

- Display the first 5 rows of the dataframe
print(df.head())

- Summary statistics
print(df.describe())

- Checking for missing values
print(df.isnull().sum())

- Visualizing the data - displot
plot = sns.displot(df['ColumnName'])
plt.show()

- Visualizing the data - boxplot
sns.boxplot(x=df['ColumnName'])
plt.show()
