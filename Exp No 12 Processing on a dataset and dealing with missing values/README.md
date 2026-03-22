Experiment – 12

Name :- Parth Dahiwade

PRN:- 25070123177

Branch:- ENTC A3

Title: Data Preprocessing and Handling Missing Values in Python

___

Aim

To understand and apply data preprocessing techniques, and to handle missing values in datasets using various Python functions and operations.

___

Theory

1. What is Data Preprocessing?

Data preprocessing is the process of cleaning, organizing, and transforming raw data into a structured format before analysis or model building.

In real-world scenarios, data is rarely perfect. It often contains errors, inconsistencies, or incomplete values that can affect the accuracy of results.

Common issues in raw datasets include:

Missing values

Incorrect or inconsistent data formats

Duplicate records

Noisy or irrelevant data

👉 Proper preprocessing ensures that the data is reliable, consistent, and ready for analysis or machine learning tasks.

2. Understanding Missing Values

Missing values are one of the most common problems in datasets. They occur when no data is stored for a particular observation.

Missing values can appear as:

NaN (Not a Number)

NULL

Blank or empty cells

Special symbols like ?, -, or NA

👉 Handling missing values is important because they can lead to incorrect conclusions or errors during analysis.

3. Data Preprocessing Functions / Operations

1. Display First Records

Used to view the top rows of the dataset for quick inspection.

👉 Function: head()

2. Display Last Records

Used to view the last few rows of the dataset.

👉 Function: tail()

3. Display Dataset Information

Provides a summary of the dataset including:

Number of rows and columns

Data types of each column

Count of non-missing values

👉 Function: info()

4. Check Data Types

Helps identify the type of data stored in each column (int, float, object, etc.).

👉 Function: dtypes

5. Identify Missing Values

Detects missing values in the dataset and returns True where values are missing.

👉 Function: isnull()

6. Count Missing Values

Calculates the total number of missing values in each column.

👉 Function: isnull().sum()

7. Detect Non-Missing Values

Returns True for valid (non-missing) data points.

👉 Function: notnull()

8. Replace Missing Symbols

Sometimes missing values are represented using symbols like ? or -. These must be converted into a standard format (NaN) for 
proper handling.

👉 Function: replace()

4. Methods to Handle Missing Values

1. Remove Rows with Missing Values

Deletes rows that contain missing data.

👉 Function: dropna()

✔ Useful when missing data is very small compared to dataset size.

2. Remove Columns with Missing Values

Deletes entire columns that contain missing values.

👉 Function: dropna(axis=1)

✔ Used when a column has too many missing values.

3. Fill Missing Values

Replaces missing values with a specified value.

👉 Function: fillna()

4. Replace with Mean

Used for numerical data by replacing missing values with the average of the column.

👉 Functions: mean() + fillna()

✔ Best when data is evenly distributed.

5. Replace with Median

Replaces missing values with the middle value of the dataset.

👉 Functions: median() + fillna()

✔ Useful when data contains outliers.

6. Replace with Mode

Replaces missing values with the most frequently occurring value.

👉 Functions: mode() + fillna()

✔ Ideal for categorical data.

7. Forward Fill Method

Fills missing values using the previous available value.

👉 Function: fillna(method='ffill')

8. Backward Fill Method

Fills missing values using the next available value.

👉 Function: fillna(method='bfill')

5. Other Important Preprocessing Operations

Remove Duplicate Records

Eliminates repeated rows to maintain data accuracy.

👉 Function: drop_duplicates()

Count Unique Values

Counts distinct values present in a column.

👉 Function: nunique()

Display Unique Values

Shows all unique categories or values in a dataset.

👉 Function: unique()

___

Conclusion

Data preprocessing is a crucial step in data analysis and machine learning. It ensures that the dataset is clean, consistent, and reliable.

___
Handling missing values properly improves the quality of analysis and leads to more accurate results. Python provides powerful tools like Pandas functions to efficiently preprocess data and deal with missing values in a systematic way.
