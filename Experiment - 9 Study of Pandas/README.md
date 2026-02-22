#Parth Dahiwade

EnTC A3 | PRN: 25070123177

Experiment - 9 Study of Pandas Library in Python

___

Aim

The aim of this project is to study the Pandas library in Python and understand how it is used for data manipulation and analysis. This includes creating Series and DataFrames, reading and writing data files, selecting and filtering data, handling missing values, performing statistical operations, and grouping and sorting data.

___

Introduction

Pandas is one of the most important Python libraries for data analysis and data manipulation. It provides two powerful data structures — Series for one-dimensional data and DataFrame for two-dimensional tabular data — that make working with structured information far more intuitive than doing it from scratch.

Pandas is built on top of NumPy, which gives it a strong numerical foundation while adding the labeling, indexing, and file-handling capabilities that raw NumPy lacks. It's widely used across data science, machine learning, finance, and business analytics, and it handles everything from small in-memory tables to large CSV files and database exports with equal ease.

___

Theory

1. Importing Pandas

Like NumPy, Pandas is imported with a standard alias that keeps code clean and concise:
pythonimport pandas as pd

The alias pd is a convention followed universally — you'll see it in virtually every data science notebook or script.

2. Pandas Series

A Series is a one-dimensional labeled array that can hold data of any type — integers, strings, floats, and so on. Think of it as a single column from a spreadsheet, but with an index attached to each value.
pythonimport pandas as pd

data = pd.Series([10, 20, 30, 40])

print(data)

Every Series has two components: its values and its index. By default the index is just 0, 1, 2... but you can assign 

meaningful labels instead:

pythonpd.Series([10, 20, 30], index=["a", "b", "c"])

This makes it easy to look up values by name rather than just position.

3. Pandas DataFrame

A DataFrame is a two-dimensional, table-like data structure with labeled rows and columns. If you've ever worked with an 

Excel sheet or a SQL table, a DataFrame will feel immediately familiar.

pythondata = {
"Name": ["A", "B", "C"],
    "Marks": [85, 90, 88]
}

df = pd.DataFrame(data)
print(df)

Each column in a DataFrame is actually a Series, which means all the properties of Series apply column-by-column inside a DataFrame as well.

4. Reading Data from CSV Files

Rather than typing data in manually, most real-world work involves loading it from external files. Pandas makes this a single line:
pythondf = pd.read_csv("file.csv")
Once loaded, a few functions help you get your bearings quickly:

df.head() — shows the first 5 rows so you can see what you're working with

df.tail() — shows the last 5 rows

df.info() — gives a summary of column names, data types, and non-null counts

df.describe() — produces a statistical summary of all numerical columns at once


5. Data Selection and Indexing

Pandas gives you two main ways to select data, each suited to different situations.

loc selects by label — meaning the actual row or column name:

pythondf.loc[0]

iloc selects by position — meaning the numeric index regardless of labels:

pythondf.iloc[0]

Selecting a single column is straightforward:

pythondf["Marks"]

And you can grab multiple columns by passing a list:

pythondf[["Name", "Marks"]]

6. Filtering Data

Filtering lets you pull out only the rows that meet a certain condition, rather than looking through everything manually:
pythondf[df["Marks"] > 85]
This returns only the rows where the Marks column exceeds 85. You can chain multiple conditions together using & (and) or | (or) for more complex filters.

7. Handling Missing Values

Real datasets are rarely perfect — values go missing for all kinds of reasons. Pandas has a set of tools specifically for dealing with this:

df.isnull() — returns a True/False mask showing where values are missing

df.notnull() — the opposite

df.dropna() — removes any row that contains a missing value

df.fillna() — replaces missing values with something you specify

For example, replacing all missing values with zero:

pythondf.fillna(0)

Which approach you choose depends on the situation — sometimes dropping rows makes sense, other times filling them in with a mean or default value is more appropriate.

8. Sorting Data

Sorting a DataFrame by a column is simple and readable:

pythondf.sort_values("Marks")

You can also sort by multiple columns at once, which is useful when the first column has ties:
pythondf.sort_values(["Marks", "Name"])

By default it sorts in ascending order, but passing ascending=False flips it.

9. GroupBy Operations

GroupBy is one of the most powerful features in Pandas. It splits your data into groups based on a column, applies a function to each group, and combines the results:

pythondf.groupby("Department").mean()

This gives you the average of every numerical column, broken down by department. It's the kind of operation that would take many lines of manual code but becomes a single readable expression in Pandas.

10. Descriptive Statistics

Pandas comes with built-in statistical functions that work directly on DataFrames and Series:

df.mean() — average

df.sum() — total

df.min() / df.max() — smallest and largest values

df.count() — number of non-null entries

df.std() — standard deviation

For example, finding the average marks across all students:

pythondf["Marks"].mean()
These can be applied to an entire DataFrame or to a specific column, giving you flexibility in how you explore your data.

Advantages of Pandas

Pandas makes data handling straightforward and readable, provides powerful tools for manipulation and aggregation, handles large datasets efficiently, integrates naturally with NumPy and Matplotlib, and is considered an essential skill for anyone working in data science.

Disadvantages

It does require installation as an external library, can consume significant memory when working with very large datasets, and has a learning curve for beginners — particularly around indexing, which can behave in unexpected ways until you understand loc vs iloc.

Tools Used

Python Interpreter, Jupyter Notebook, VS Code / IDLE, and the Pandas library itself.

Applications

Pandas is used in data cleaning, exploratory data analysis, financial modeling, business reporting, preprocessing data for machine learning, and academic research and statistics.

___

Conclusion

Pandas is a flexible and genuinely indispensable library for data work in Python. Through this study, we covered how to create Series and DataFrames from scratch, load real datasets from CSV files, filter and manipulate data using conditions, deal with missing values gracefully, and apply statistical functions with minimal code.

A strong grasp of Pandas is the natural bridge between knowing Python basics and being able to do meaningful work in data science, machine learning, and analytics. Most data pipelines and notebooks you'll encounter in the wild will have Pandas at their core.
