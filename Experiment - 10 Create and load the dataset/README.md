Parth Dahiwade

EnTC A3 | PRN: 25070123177

Experiment 10: Creating and Uploading a Dataset using Pandas

___

Aim

To create a dataset in Python and perform basic data inspection operations such as size, shape, info, and describe using Pandas.

Objectives

To create a dataset using a dictionary

To convert it into a DataFrame

To upload and read a dataset from a CSV file

To perform basic data analysis using shape, size, info(), describe(), head(), and tail()



Software Requirements

Python 3.x
Pandas library
Jupyter Notebook / Google Colab / Python IDE

___

Theory

A dataset is simply a collection of related data organized in a structured way. In Pandas, datasets are stored as DataFrames — two-dimensional tables with labeled rows and columns, much like a spreadsheet.

Datasets can either be created manually within the code itself, or loaded from external files. Pandas supports a wide range of file formats for this, including CSV, Excel, JSON, and SQL databases.

Once a dataset is loaded, the first thing you typically want to do is inspect it — understand its structure, check for missing values, see what data types are present, and get a quick statistical summary. Pandas provides a set of built-in functions that make this initial exploration quick and straightforward.

Basic Inspection Functions
FunctionPurposedf.shapeNumber of rows and columnsdf.sizeTotal number of elementsdf.info()Structure of the dataset including data types and null countsdf.describe()Statistical summary of numerical columnsdf.head()First 5 rowsdf.tail()Last 5 rowsdf.columnsList of all column names

___

Program
Part A: Creating the Dataset
We start by defining the data as a Python dictionary, where each key becomes a column name and each list becomes the column's values. This is then passed into pd.DataFrame() to create the structured table.
pythonimport pandas as pd

data = {
    "Roll_No": [101, 102, 103, 104, 105],
    "Name": ["Amit", "Neha", "Rohit", "Sneha", "Kiran"],
    "Marks": [85, 90, 78, 88, 76],
    "Department": ["IT", "CS", "IT", "ENTC", "CS"]
}

df = pd.DataFrame(data)
print(df)

Part B: Basic Dataset Inspection
With the DataFrame created, we can now run through the core inspection functions to understand what we're working with.
pythonprint("Shape:", df.shape)
print("Size:", df.size)
print("\nColumn Names:\n", df.columns)
print("\nFirst 5 rows:\n", df.head())
print("\nLast 5 rows:\n", df.tail())
print("\nDataset Info:\n")
df.info()
print("\nStatistical Summary:\n", df.describe())
df.shape tells us the dataset has 5 rows and 4 columns. df.size gives the total element count, which is 20 (5 × 4). df.info() shows the column names, their data types, and whether any values are missing. df.describe() gives a statistical breakdown — mean, standard deviation, min, and max — for the numerical column Marks.

Part C: Saving the Dataset to a CSV File
Once the DataFrame is ready, saving it as a CSV file is a single line. The index=False argument prevents Pandas from writing the row numbers into the file, keeping it clean.
pythondf.to_csv("students.csv", index=False)

Part D: Reading the Dataset Back from CSV
To simulate loading an external dataset — the way you would in a real project — we read the saved CSV file back into a new DataFrame and print it to confirm everything was stored correctly.
pythondf2 = pd.read_csv("students.csv")
print("\nUploaded Dataset:\n", df2)

Output

Dataset created successfully and displayed as a formatted table
Shape returned as (5, 4) and size as 20
Column names listed correctly
info() confirmed data types and showed no missing values
describe() generated statistical summary for the Marks column
CSV file saved and read back successfully with all data intact

___

Conclusion

In this experiment, we created a structured student dataset using a Python dictionary and converted it into a Pandas DataFrame. We then explored it using the core inspection functions — shape, size, info(), and describe() — which together give a complete picture of any dataset's structure and content. Finally, we saved the DataFrame as a CSV file and read it back, demonstrating how Pandas handles the full cycle of creating, storing, and loading data. These are foundational skills that apply directly to any real-world data analysis or machine learning workflow.
