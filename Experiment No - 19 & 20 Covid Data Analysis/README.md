
🦠 COVID-19 Intelligence & Global Trends Analysis


Title :- Exploratory Data Analysis | Experiment 19 & 20

👤 Name:   Parth Dahiwade 

🆔 PRN: 25070123177

🏛️ Batch: EnTC A3

___

📄 Theory :-

This project presents a computational analysis of the COVID-19 pandemic using Python-based data science tools. A multi-dimensional time-series dataset (January 2020 – May 2021) is analyzed through data cleaning, feature engineering, and visualization techniques.

The study focuses on understanding global infection trends, detecting inconsistencies in reporting, and evaluating healthcare outcomes at both global and regional levels.

___

🎯 Project Objectives

Data Cleaning & Preparation

Removed unnecessary columns (SNo, Last Update) and converted date fields into proper datetime format for time-series analysis.

Feature Engineering

Created new metrics such as:

Active Cases

Mortality Rate (%)

Recovery Rate (%)

These enable meaningful comparison across countries.

Geospatial Analysis

Built interactive choropleth maps using Plotly to visualize the global spread of COVID-19.

Trend Smoothing

Applied 7-day rolling averages to eliminate irregularities like reporting delays and weekend effects.

Hotspot Identification

Analyzed region-level data (Spain) to identify high-risk areas using aggregation techniques.

___

🛠️ Tools & Technologies

Category	Tools	Key Uses

Data Processing	Pandas, NumPy	Data cleaning, aggregation, transformations

Visualization	Matplotlib, Seaborn	Graphs, heatmaps

Interactive Mapping	Plotly Express	Choropleth maps

Platform	Jupyter Notebook / Colab	Execution & visualization

___

📊 Methodology & Key Insights

1. Data Preprocessing

Inspected dataset using .info() and .head()

Handled missing values

Converted numerical columns for accuracy

Cleaned redundant attributes

2. Global Trend Analysis (Experiment 19)

Filtered latest data snapshot (May 29, 2021)

Aggregated country-level data using groupby()

Generated global distribution insights

3. Advanced Insights

Reporting Anomaly Detection

The US showed 0% recovery rate due to reporting changes—not actual data.

Wave Pattern Analysis

Identified India’s second wave peak (April 2021) using rolling averages.

Correlation Study

Heatmap analysis revealed:

Strong correlation (~0.95) between confirmed cases and deaths

Mortality depends more on healthcare quality than case count

4. Spain Regional Analysis (Experiment 20)

Studied province-level data

Used groupby() and idxmax() to detect hotspots

Visualized results using a choropleth map

___

🏁 Conclusion

This project demonstrates how Python can transform raw pandemic data into meaningful insights. By applying normalization and smoothing techniques, the analysis provides a clearer understanding of global health patterns.
