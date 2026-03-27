Parth Dahiwade

ENTC A3 | PRN: 25070123177

Experiment – 13

Title: Data Binning and Data Formatting in Python

___

Aim

To understand and perform data binning and data formatting using Python tools and functions.

___

Theory

In real-world data analysis, raw data is often messy and unorganized. Before we can analyze it properly, we need to clean and structure it — this process is called data preprocessing.

Two important techniques used in preprocessing are:

1. Data Binning

Data binning means grouping continuous numerical values into categories or ranges (bins).

This helps to:

Reduce noise and small fluctuations in data

Make patterns easier to understand

Convert continuous data into categorical data

Example:

Age	Category

18	Young

30	Adult

60	Senior

Instead of dealing with exact ages, we group them into meaningful categories.

2. Data Formatting

Data formatting involves converting data into a consistent and usable format so it can be easily processed and analyzed.

Common formatting tasks include:

Converting text into numbers

Changing date formats

Standardizing text (uppercase/lowercase)

Removing unnecessary spaces

Proper formatting improves accuracy, readability, and consistency of data.

Functions Used for Data Binning

Creating Bins

pd.cut()

Used to divide data into equal-sized intervals.

Quantile-Based Binning

pd.qcut()

Divides data so that each bin has an equal number of observations.

Counting Values in Each Bin

value_counts()

Displays how many values fall into each category.

Custom Labels for Bins

labels

Assigns meaningful names to bins such as:

Low

Medium

High

Functions Used for Data Formatting

Checking Data Types

dtypes

Helps identify the type of data in each column.

Changing Data Types

astype()

Converts data from one type to another (e.g., string to integer).

Converting Strings to Numbers

pd.to_numeric()

Useful when numeric data is stored as text.

Working with Dates

pd.to_datetime()

Converts data into proper date format.

Text Formatting

str.lower() → converts text to lowercase

str.upper() → converts text to uppercase

str.title() → capitalizes each word

Removing Extra Spaces

str.strip()

Removes unwanted spaces from the beginning and end.

Replacing Values

replace()

Used to correct or standardize inconsistent values.

___

Conclusion

In this experiment, we learned how to organize and clean data using data binning and formatting techniques in Python. These methods make data easier to analyze and improve the overall quality and reliability of results.

___
