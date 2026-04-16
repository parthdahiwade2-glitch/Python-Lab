📈 Statistical and Specialized Data Visualization in Python

Name: Parth Dahiwade

Branch: EnTC A3

PRN: 25070123177

___

📄 Experiment Title

Exploring Statistical and Specialized Data Visualization Techniques

___

🎯 Objective

To study and implement advanced data visualization techniques such as Heatmaps, Boxplots, Area Plots, and Bubble Charts for analyzing distributions, detecting outliers, identifying correlations, and representing multi-dimensional data.

___

📌 Overview

Statistical visualization helps in summarizing complex datasets and uncovering hidden patterns. This experiment focuses on:

Distribution & Outliers: Using boxplots and histograms

Proportions: Using pie and donut charts

Correlations: Using heatmaps to analyze relationships between variables

Multi-dimensional Data: Using bubble plots to represent multiple variables simultaneously

___

🧠 Key Concepts

1. Area Plot


An area plot is similar to a line chart but fills the area beneath the curve.

Use: To represent cumulative values or compare quantities (e.g., Sales vs Profit).

2. Boxplot (Whisker Plot)

Displays data distribution using the five-number summary:

Minimum, Q1, Median, Q3, Maximum.

Use: Detecting outliers and understanding data spread.

3. Heatmap

Represents data values using color intensity.

Use: Visualizing correlation matrices to understand relationships between variables.

4. Bubble Plot

An extension of scatter plots where:

Size → represents third variable

Color → represents fourth variable

Use: Visualizing multi-dimensional datasets effectively.

___

⚙️ Procedure

Library Initialization:

Import required libraries:

matplotlib.pyplot, seaborn, pandas, numpy

Dataset 1 (Categorical Data):

Create a dataset with categories (A–E)

Use it for pie charts, donut charts, and basic plots

Advanced Visualization:

Create exploded pie charts

Construct donut charts using circular overlays

Generate correlation heatmaps using .corr()

Dataset 2 (Numerical Data):

Generate synthetic dataset (Age, Income, Loan Amount, Credit Score)

Perform statistical analysis

Statistical Analysis:

Detect outliers using boxplots

Analyze distribution using histograms

___

📘 Implementation Highlights

🔹 Correlation Heatmap

corr = df[['Age','Income','Loan_Amount','Credit_Score']].corr()

sns.heatmap(corr, annot=True, cmap='coolwarm')

🔹 Donut Chart

plt.pie(df['Values'], labels=df['Category'], autopct='%1.2f%%')

centre_circle = plt.Circle((0,0), 0.4, fc='white')

fig = plt.gcf()

fig.gca().add_artist(centre_circle)

🔹 Bubble Plot (Seaborn)

sns.scatterplot(

    x='Sales', 
    
    y='Profit', 
    
    size='Values', 
    
    hue='Values', 
    
    data=df, 
    
    sizes=(50, 300)
)


___

📋 Key Functions Used

Function	Library	Purpose

plt.fill_between()	Matplotlib	Creates area plots

plt.pie()	Matplotlib	Creates pie charts

sns.boxplot()	Seaborn	Detects outliers

.corr()	Pandas	Computes correlation matrix

sns.heatmap()	Seaborn	Displays correlation visually

plt.Circle()	Matplotlib	Creates donut chart effect

___

📊 Dataset Observations

Outliers: Boxplots help identify extreme loan amounts.

Correlation: Heatmaps reveal relationships between income, credit score, and loan amount.

Distribution: Histograms indicate whether data is normally distributed or skewed.

___

🎯 Outcome

Implemented advanced visualization techniques effectively

Learned to interpret correlations using heatmaps

Identified outliers using boxplots

Visualized multi-variable data using bubble plots

Improved understanding of visualization aesthetics (color palettes, transparency)

___

📌 Conclusion


Statistical visualizations play a crucial role in deeper data analysis. Unlike basic charts, these techniques provide insights into data distribution, relationships, and anomalies. This experiment demonstrated how advanced plots like heatmaps and boxplots enhance exploratory data analysis (EDA), making them essential tools in data science and machine learning.
