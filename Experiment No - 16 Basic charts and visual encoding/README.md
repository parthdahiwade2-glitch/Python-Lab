📄 Experiment No - 16

Name :- Parth Dahiwade

PRN:- 25070123177

Branch:- ENTC A3

___

Title: Categorical Data Analysis using Python

Data Visualization using Matplotlib and Seaborn

___

🎯 Objective

To study and implement basic data visualization techniques using Matplotlib and Seaborn for representing numerical and categorical data, and to analyze trends, comparisons, distributions, and relationships.

___

📌 Overview

Data visualization refers to the graphical representation of data using visual elements such as charts and graphs. It helps in understanding patterns, trends, and outliers effectively.

Matplotlib: A low-level Python library used for creating detailed and customizable plots.

Seaborn: A high-level library built on Matplotlib that provides attractive and informative statistical visualizations with simpler syntax.

🧠 Key Concepts

Visual Encoding: Representing data using visual properties like color, size, and position.

Trend Analysis: Identifying patterns over time using line charts.

Categorical Comparison: Comparing discrete categories using bar charts.

Distribution: Understanding frequency of values using histograms.

Correlation: Identifying relationships between variables using scatter plots.

___

📘 Theory & Visualizations

1. Line Charts (Trend Analysis)

Line charts display data points connected by straight lines.

Use: To show continuous changes over time (e.g., daily study hours).

2. Bar Charts (Comparison)

Bar charts represent categorical data using rectangular bars.

Simple Bar Chart: Compares single variable across categories.

Grouped Bar Chart: Compares multiple variables across categories.

3. Histograms (Distribution)

Histograms group data into bins to represent frequency distribution.

Alpha Parameter: Controls transparency of bars.

4. Scatter Plots (Correlation)

Scatter plots show relationships between two numerical variables.

Conditional Encoding: Different colors represent additional categories (e.g., Pass/Fail).

___

⚙️ Procedure

Setup Environment:

Import required libraries:

matplotlib.pyplot, seaborn, pandas, numpy

Data Preparation:

Create dataset (Days, Marks, Study Hours, Attendance).

Convert data into a Pandas DataFrame.

Matplotlib Visualization:

Plot line charts with markers and styles.

Create bar charts with value annotations.

Generate histograms for distribution analysis.

Plot scatter graphs with conditional coloring.

Seaborn Visualization:

Load secondary dataset (e.g., Sales and Profit).

Create line plots, bar plots, and scatter plots with simplified syntax.

📘 Implementation Highlights

🔹 Adding Labels to Bar Chart

bars = plt.bar(df['Days'], df['Marks'], color='cyan')

for bar in bars:

    y = bar.get_height()
   
    plt.text(bar.get_x() + bar.get_width()/2, y, str(y), 
    
             ha='center', va='bottom')

🔹 Grouped Bar Chart

x = np.arange(len(df['Days']))

width = 0.35

plt.bar(x - width/2, df['Study_Hours'], width, label='Study Hours')

plt.bar(x + width/2, df['Marks'], width, label='Marks')

🔹 Seaborn Plots

sns.lineplot(x='Day', y='Sales', data=df)

sns.scatterplot(x='Sales', y='Profit', data=df)

📋 Key Functions Used

Function	Library	Description

plt.plot()	Matplotlib	Creates line charts

plt.bar()	Matplotlib	Creates bar charts

plt.hist()	Matplotlib	Creates histograms

plt.scatter()	Matplotlib	Creates scatter plots

plt.legend()	Matplotlib	Adds legend to graph

sns.barplot()	Seaborn	Creates aesthetic bar charts

plt.xticks()	Matplotlib	Sets x-axis labels

📂 Applications

Academic Analysis: Comparing study hours with marks.

Business Analysis: Tracking sales and profit trends.

Data Science: Performing exploratory data analysis (EDA).

🎯 Outcome

Learned to create and customize various plots.

Gained understanding of multiple data visualization techniques.

Successfully implemented grouped charts using NumPy.

Utilized Seaborn for efficient and visually appealing plots.

___

📌 Conclusion

Data visualization plays a crucial role in analyzing and interpreting data. This experiment demonstrated the effective use of Matplotlib for detailed customization and Seaborn for quick and aesthetically pleasing visualizations, providing a strong foundation for data analysis tasks.
