# Python Part 3
This week, we have learned more about python which includes:
## Numpy
NumPy is a Python library that provides support for large, multi-dimensional arrays and matrices, along with a collection of mathematical functions to operate on these arrays. Arrays are efficient and fast for numerical operations. They enable you to work with large datasets more easily than standard Python lists.

### Dimmension
In NumPy, the term "dimension" refers to the number of axes or directions in which data can vary. In NumPy, the ‘ndmin’ parameter is used when creating an array to specify the minimum number of dimensions that the resulting array should have. It allows you to explicitly set the number of dimensions. 

![dimensi](https://github.com/pritaaa/Python-Part-3/assets/96106020/198d1ab4-d91d-4e42-bb29-7da18c23bf37)

From the example above, we call 7 dimensions with the expression 'ndmin=7' where the number 7 can be filled as desired.

## Pandas
Pandas is a Python library for efficient data manipulation and analysis. It simplifies data cleaning, transformation, and analysis tasks with its DataFrame and Series data structures. Pandas are widely used in data science to handle structured data, perform statistical operations, and work with various file formats.
### Object Series
A Pandas Series is like a column in a table. It is a one-dimensional array holding data of any type. It is similar to a column in a table and can be thought of as a fixed-size dictionary, where the index labels map to the corresponding values.

![objct](https://github.com/pritaaa/Python-Part-3/assets/96106020/35caa08f-254a-4923-ba1d-2d9614fa427b)

### Data Slicing
Slicing allows to select specific rows or columns from the data structure based on their labels or positions.
#### Explicit and Implicit Data Index
Explicit data slicing retrieves a subset of data with reference to an explicitly specified index, such as an index range or a specific index. An implicit data slicing retrieves a subset of data with reference to an implicitly specified index, such as a specific rule or condition where the last index is not included in the resulting subset of data.

![index](https://github.com/pritaaa/Python-Part-3/assets/96106020/ad2ef2c0-e211-4279-961c-480a10be92fd)

#### Loc &Iloc
Loc calls an explicit index and an Iloc calls an implicit index. Loc and iloc used to remove inconsistencies in data slicing.

![loc iloc](https://github.com/pritaaa/Python-Part-3/assets/96106020/5a80ad65-4b3b-48d9-8b07-f352a9fc1d27)


## DataFrame
DataFrame is a collection of series with at least 1 series. A DataFrame in Python is a two-dimensional, size-mutable, and potentially heterogeneous tabular data structure with labeled axes (rows and columns). It can be thought of as a table with rows and columns. In example, DataFrame builded by 3 series.

![df1](https://github.com/pritaaa/Python-Part-3/assets/96106020/9f2cb969-b96f-4b3a-b242-528b9275ef5f)

![df2](https://github.com/pritaaa/Python-Part-3/assets/96106020/4ec83d2c-e551-44ae-bcb9-21124c531e16)

## Load Data CSV in Pandas
To import a CSV file in Python, you can use the Pandas library, which provides a simple and efficient way to work with structured data. Make sure csv data that has been aplouded in the same folder. 

![csv1](https://github.com/pritaaa/Python-Part-3/assets/96106020/4c5df245-0c44-46c5-af5e-3830eded12ca)

Given example of importing data 'Titanic.csv' with the “pd.read_csv()” function.
### Head
•	viewing from top data
•	can be customized
•	head by default is top 5

![head](https://github.com/pritaaa/Python-Part-3/assets/96106020/8871e2e4-3ae3-4f77-84bb-11c900456085)

### Tail
•	tail()returns a specified number of last rows.
•	tail()returns the last 5 rows if a number is not specified.

![tail](https://github.com/pritaaa/Python-Part-3/assets/96106020/aa8b9370-df69-455d-95a2-494261bda736)
 
### Info
•	info() method prints information about the DataFrame.
•	The information contains the number of columns, column labels, column data types, memory usage, range index, and the number of cells in each column (non-null values).

![info](https://github.com/pritaaa/Python-Part-3/assets/96106020/305b15d8-8e73-4f0b-8643-02dc08427f1e)

### shape
shape is the number of rows and columns of the DataFrame.

![shape](https://github.com/pritaaa/Python-Part-3/assets/96106020/df1bf184-f57c-4a59-87b0-77e531dbd04e)

891 is the number of rows, 12 is the number of columns
### columns
columns returns the label of each column in the DataFrame.

![columns](https://github.com/pritaaa/Python-Part-3/assets/96106020/efbbc336-5398-4eff-9d98-ee3ec3359a42)

### index
•	The index returns the index information of the DataFrame.
•	The index information contains the labels of the rows. If the rows has NOT named indexes, the index property returns a RangeIndex object with the start, stop, and step values.

### sum
•	Returns the sum of the values in the specified axis
•	The sum() method adds all values in each column and returns the sum for each column.
•	By specifying the column axis (axis='columns'), the sum() method searches column-wise and returns the sum of each row.
### isnull
Isnull used to finds NULL values.

![isnull](https://github.com/pritaaa/Python-Part-3/assets/96106020/b5bc4b6e-87ac-4fb2-8b8b-2552bedf1aaa)

### notnull
Notnull used to finds values that are NOT NULL.

![notnull](https://github.com/pritaaa/Python-Part-3/assets/96106020/730a419f-8034-40b3-ac8c-d43a570be5e4)

### describe
Returns a description summary for each column in the DataFrame

![image](https://github.com/pritaaa/Python-Part-3/assets/96106020/79db4aa9-ed7d-4e48-9752-8006b38b69fc)

### mean
•	Return the mean of the values in the specified axis
•	Mean: The average value
### median
•	Median: The mid point value
•	Return the median of the values in the specified axis
### mode
•	Mode: The most common value
•	Returns the mode of the values in the specified axis
### min
Returns the min of the values in the specified axis
### max
Return the max of the values in the specified axis
