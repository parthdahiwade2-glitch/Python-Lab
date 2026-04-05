Experiment No - 14

Name :- Parth Dahiwade

PRN:- 25070123177

Branch:- ENTC A3

Title: Data Normalization and Turning Categorical Variables into Quantitative Variables in Python

___

Aim

To study and perform data normalization and convert categorical variables into quantitative variables using various Python functions and operations.

___

Theory

In real-world data analysis and machine learning, raw data is rarely clean or ready to use. It often contains values that vary widely in scale and includes categorical (non-numeric) information. If such data is used directly, it can lead to incorrect analysis or poor model performance.

To overcome this, data preprocessing is an essential step. It ensures that the dataset becomes structured, consistent, and suitable for computational models.

Two important preprocessing techniques are:

• Data Normalization

• Categorical Variable Encoding

These techniques improve the quality of data, ensure fairness among features, and enhance the accuracy and efficiency of analysis and machine learning models.

1. Data Normalization

Definition

Data normalization is a technique used to rescale numerical data into a common range so that all features contribute equally to the analysis.

In many datasets, different features have different ranges. For example:

Feature	Range

Price	500 – 50000

Rating	1 – 5

Units Sold	10 – 1000

If normalization is not applied, features like Price (large values) will dominate features like Rating (small values), 
leading to biased results.

Why Normalization is Important

Normalization helps to:

• Bring all features to the same scale

• Prevent dominance of large-value features

• Improve the performance of machine learning algorithms

• Make comparisons between variables easier and meaningful

Types of Normalization

1. Min-Max Normalization

This method scales all values between 0 and 1.

It works by subtracting the minimum value and dividing by the range of the dataset. This ensures all values lie within a fixed interval.

Functions / Operations Used:

• min() → Finds the smallest value

• max() → Finds the largest value

2. Z-score Normalization (Standardization)

This method transforms data based on its mean (average) and standard deviation.

It tells how far a value is from the average in terms of standard deviations.

• Values near 0 → Close to mean

• Positive values → Above mean

• Negative values → Below mean

Functions / Operations Used:

• mean() → Calculates average

• std() → Calculates standard deviation

3. Decimal Scaling

In this method, values are scaled by shifting the decimal point.

This is done by dividing values by powers of 10 until all values fall within a smaller range (typically between -1 and 1).

Operation Used:

• Division by powers of 10

Useful Functions for Normalization
Summary Statistics

describe()
This function provides a quick statistical summary of the dataset, including:

• Mean

• Standard deviation

• Minimum value

• Maximum value

Identify Data Types

dtypes

Used to identify which columns are numerical and need normalization.

Select Columns

• loc[] → Label-based selection

• iloc[] → Index-based selection

These are used to apply normalization only to selected columns.

2. Turning Categorical Variables into Quantitative Variables

Definition

Categorical variables represent qualitative data, which cannot be directly used in mathematical models.

Examples:

Variable	Values

Gender	Male, Female

Payment Method	UPI, Debit Card

Product Category	Electronics, Clothing

Since most data analysis and machine learning algorithms require numerical input, categorical data must be converted into numeric form.

This process is called categorical encoding.

Methods to Convert Categorical Data

1. Label Encoding

In this method, each category is assigned a unique numerical value.

Example:

Category	Encoded Value

Male	0

Female	1

This method is simple but may introduce unintended ordering between categories.

Functions / Operations Used:

• LabelEncoder()

• fit_transform()

2. One-Hot Encoding

This method creates separate binary (0 or 1) columns for each category.

Example:

Category	Electronics	Clothing	Home

Electronics	1	0	0

This method avoids ranking issues and is widely used in machine learning.

Functions / Operations Used:

• get_dummies()

3. Dummy Encoding

This is similar to One-Hot Encoding, but one column is removed to avoid redundancy and multicollinearity.

This helps in improving model efficiency without losing information.

Functions / Operations Used:

• get_dummies(drop_first=True)

___

Conclusion

In this experiment, data normalization and categorical variable transformation techniques were studied and understood in detail. These preprocessing methods play a crucial role in preparing raw data for analysis and machine learning. By applying normalization, numerical features are scaled effectively, and by encoding categorical variables, qualitative data is converted into a usable numerical format. Overall, these techniques significantly improve the reliability, accuracy, and performance of data-driven models.

___
