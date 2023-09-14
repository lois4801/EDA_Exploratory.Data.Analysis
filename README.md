# EDA_Exploratory.Data.Analysis

## Good books
https://www.oreilly.com/library/view/hands-on-exploratory-data/9781789537253/

https://www.oreilly.com/library/view/hands-on-data-preprocessing/9781801072137/?_gl=1*4o17pe*_ga*MTY2NDExODYzOC4xNjk0NzE5MjM3*_ga_092EL089CH*MTY5NDcxOTIzNy4xLjEuMTY5NDcxOTM2NC42MC4wLjA.



**Exploratory Data Analysis (EDA)** is an approach to analyzing data sets to summarize their main characteristics, often with visual methods. Here are the steps involved in EDA:

1. Data Collection: This is the first step where you gather the data from various sources.

2. Data Cleaning: This step involves handling missing data, removing duplicates and outliers.

3. Data Wrangling or Data Munging: In this process, the raw data is transformed into another format to make it more suitable for analysis.

4. Data Analysis: In this step, various statistical techniques are used to analyze the data.

5. Data Visualization: This involves presenting your data in a visual format like graphs, charts etc., to understand the patterns, trends and insights in the data.
---------------------------------------------------------------------
### Importing required libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

### Load the dataset
df = pd.read_csv('data.csv')

### Display the first 5 rows of the dataframe
print(df.head())

### Summary statistics
print(df.describe())

### Checking for missing values
print(df.isnull().sum())

### Visualizing the data - displot
plot = sns.displot(df['ColumnName'])
plt.show()

### Visualizing the data - boxplot
sns.boxplot(x=df['ColumnName'])
plt.show()

---------------------------------------------------------------
## There are four types of Exploratory Data Analysis (EDA):

**Univariate Non-graphical:** This is the simplest form of data analysis where we use just one variable to analyze the data. The standard goal of univariate non-graphical EDA is to understand the underlying sample distribution/data and make observations about the population1.

**Multivariate Non-graphical:** Multivariate non-graphical EDA technique is often used to show the relationship between two or more variables in the form of either cross-tabulation or statistics1.

**Univariate Graphical:** This involves visualizing a single variable’s data distribution using graphical methods like histograms, box plots, etc1.

**Multivariate Graphical:** This involves visualizing relationships between multiple variables using graphical methods like scatter plots, pair plots, etc1.

Effectivitiy depends on the specific scenario and what you’re trying to achieve with your analysis. Each type has its own strengths and is suited to different kinds of data and different questions.
For example, if you’re trying to understand the distribution of a single variable, univariate graphical or non-graphical might be most effective. If you’re trying to understand relationships between variables, multivariate graphical or non-graphical might be more appropriate.

It’s also worth noting that these types are not mutually exclusive and can be used in combination during an EDA process. The key is to choose the right approach based on your data and your analysis goals.










