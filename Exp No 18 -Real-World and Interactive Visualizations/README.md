🌐 Real-World and Interactive Visualizations

Name: Parth Dahiwade

Branch: EnTC A3

PRN: 25070123177

___

📄 Experiment Title

Advanced Visualizations: Hierarchical, Interactive, and Multi-dimensional Charts

___

🎯 Objective

To implement advanced and interactive data visualization techniques using Plotly, SciPy, and Matplotlib-Venn for representing hierarchical structures, process flows, and multi-dimensional datasets.

___

📌 Overview

Traditional 2D charts are often limited in representing complex datasets. This experiment focuses on advanced visualization techniques to enhance data storytelling:

Interactive Visualizations: Using Plotly for zooming, hovering, and rotation

Hierarchical Data Representation: Using treemaps and dendrograms

Process Flow Visualization: Using Sankey diagrams

Set Relationships: Using Venn diagrams

___

🧠 Key Concepts

1. Treemap

Treemaps use nested rectangles to represent hierarchical data.

Use: Visualizing proportions within categories (e.g., budget allocation, storage usage).

2. Dendrogram

A tree-like diagram used in hierarchical clustering.

Use: Identifying cluster relationships and optimal grouping.

3. Sankey Diagram

A flow diagram where the width of connections represents quantity.

Use: Tracking transitions such as student progression or energy flow.

4. Radar (Spider) Chart

Displays multivariate data across multiple axes from a central point.

Use: Skill assessment or performance comparison.

5. 3D Scatter Plot

Extends scatter plots by adding a third axis.

Use: Analyzing relationships among three numerical variables.

___

⚙️ Procedure

Library Setup:

Import required libraries:

plotly.express, plotly.graph_objects, scipy.cluster.hierarchy, matplotlib_venn

Hierarchical Clustering:

Apply linkage method on dataset

Plot dendrogram to visualize clusters

Interactive Visualization:

Create 3D scatter plots using Plotly

Enable interactivity (zoom, rotate, hover)

Flow Representation:

Construct Sankey diagram to show data flow stages

Skill Mapping:

Use radar chart to represent multi-dimensional performance

___

📘 Implementation Highlights

🔹 3D Scatter Plot (Plotly)

fig = px.scatter_3d(df, x='Study_Hours', y='Marks', z='Attendance')

fig.show()

🔹 Hierarchical Clustering (Dendrogram)

from scipy.cluster.hierarchy import dendrogram, linkage


linked = linkage(data, method='ward')

dendrogram(linked)


___

📋 Key Functions Used

Function	Library	Purpose

px.treemap()	Plotly Express	Visualizes hierarchical data

linkage()	SciPy	Performs hierarchical clustering

venn2()	Matplotlib-Venn	Shows set intersections

go.Sankey()	Plotly	Represents flow between stages

go.Scatterpolar()	Plotly	Creates radar charts

px.scatter_3d()	Plotly	Interactive 3D visualization

___

📂 Applications

Education: Tracking student progression using Sankey diagrams

HR Analytics: Skill evaluation using radar charts

Finance: Portfolio distribution using treemaps

Biology: Classification using dendrograms

___

🎯 Outcome

Developed interactive and dynamic visualizations

Learned to represent hierarchical and flow-based data

Gained experience with multi-dimensional plotting (3D & polar)

Enhanced data storytelling for real-world applications

___

📌 Conclusion

Advanced visualization techniques provide deeper insights compared to traditional charts. This experiment demonstrated how tools like Plotly and SciPy enable the creation of interactive and high-dimensional visualizations, making data analysis more intuitive, insightful, and impactful.
