EXPERIMENT-10
STUDY OF PANDAS LIBRARY IN PYTHON
NIKUNJ DEEP UPADHYAY
ENTC B1
25070123081

EXPERIMENT 10: Study of Pandas Library in Python – Theory
1. Introduction to Pandas

Pandas is a powerful open-source Python library used for data analysis and data manipulation. It provides easy-to-use data structures and tools for handling structured data efficiently. Pandas is mainly used in:

Data analysis

Data cleaning

Data transformation

Statistical analysis

Data filtering and processing

It is especially useful for working with tabular data like spreadsheets or SQL tables.

2. Important Data Structures in Pandas

Pandas provides two main data structures:

(a) Series

A one-dimensional labeled array.

Can store data of any type (integers, strings, floats, etc.).

Each element has an index.

Example concept:
A list of marks:
[10, 20, 30, 40]
is stored as a Series with automatic indexing (0,1,2,3).

(b) DataFrame

A two-dimensional labeled data structure.

Similar to a table (rows and columns).

Columns can contain different data types.

Example structure:

NAME	MARKS
A	85
B	90
C	78

Each column is a Series, and together they form a DataFrame.

3. Creating Data Structures
Creating a Series

A Series is created using:

pd.Series()
Creating a DataFrame

A DataFrame is created using:

pd.DataFrame()

Data is generally passed as a dictionary where:

Keys = Column names

Values = Data lists

4. Properties of DataFrame
(a) shape

Returns number of rows and columns.

Format: (rows, columns)

(b) ndim

Returns number of dimensions.

DataFrame → 2 dimensions

(c) size

Returns total number of elements.

Formula:

rows × columns
(d) columns

Displays column names.

(e) dtypes

Shows data type of each column.

5. Accessing Data
(a) Accessing Columns
df["COLUMN_NAME"]
(b) Accessing Specific Elements
Using loc[]

Access by row label and column name

df.loc[row_label, "COLUMN_NAME"]
Using iloc[]

Access by row index and column index

df.iloc[row_index, column_index]
6. Modifying DataFrame
(a) Adding a New Column

A new column can be added by:

df["NewColumn"] = values
(b) Updating Data

Values can be modified using:

df.iloc[row_index, column_index] = new_value
(c) Deleting a Column

Column can be removed using:

df.drop("ColumnName", axis=1)

axis=1 means column deletion.

7. Statistical Operations in Pandas

Pandas provides built-in statistical functions:

mean() → Average value

min() → Minimum value

max() → Maximum value

These functions are applied to specific columns.

Example:

df["MARKS"].mean()
8. Data Filtering

Filtering allows selecting data based on conditions.

Example:

df[df["MARKS"] > 80]

This displays students who scored more than 80.

9. Conclusion

From this experiment, we study:

Creation of Series and DataFrame

Understanding DataFrame structure

Accessing and modifying data

Adding and deleting columns

Performing statistical operations

Applying conditional filtering

Pandas makes data handling simple, fast, and efficient, which is why it is widely used in data science, machine learning, and analytics.

