# Elevate-lab-T2

1. Data Loading and Initial Exploration

imported the pandas library using import pandas as pd.
loaded the Titanic dataset using df = pd.read_csv('/content/titanic data set.zip').
displayed the first few rows of the dataset using print(df.head()).
got an overview of the dataset using print(df.info()), which shows column names, data types, and missing values.
calculated summary statistics for numerical columns using print(df.describe()), including measures like mean, standard deviation, and quartiles.

2. Visualizing Numeric Features

 imported the matplotlib.pyplot library as plt and used it to create a histogram of the 'Age' column. This helps visualize the age distribution of passengers.
imported the seaborn library as sns and used it to create a box plot of the 'Fare' column. This helps visualize the distribution and potential outliers in ticket fares.

3. Exploring Relationships Between Features

calculated the correlation matrix using df.corr(numeric_only=True) and visualized it as a heatmap using sns.heatmap. This helps identify potential relationships between numerical features.
created a pair plot using sns.pairplot to visualize relationships between 'Age', 'Fare', 'Pclass', and 'Survived'. This helps identify clusters and trends in the data.

4. Checking Patterns and Trends

calculated the survival rate by gender using df.groupby('Sex')['Survived'].mean() and by passenger class using df.groupby('Pclass')['Survived'].mean(). This helps identify potential patterns in survival based on these categories.
created a bar plot using sns.barplot to visualize the survival rate by passenger class. This provides a visual representation of the survival rate differences between classes.

5. Interactive Plots with Plotly

imported plotly.express as px and created an interactive scatter plot using px.scatter. This plot allows users to explore the relationship between 'Age', 'Fare', 'Sex', and 'Survived' with interactive features like zooming and hovering.
