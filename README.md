# Python_Week_2

## Function
A python program is made of many lines of code, stored in a file with a name like "example.py". It's natural to have a way to divide the lines code up into sensible sub-parts, and these are called functions. Almost all the code you work with in Python is inside a function.
- A function is a block of code which only runs when it is called.
- You can pass data, known as parameters, into a function.
- In Python a function is defined using the "def" keyword
- A function can return data as a result.

![Screenshot (770)](https://github.com/Rnovranza/Python_Week_2/assets/134476980/dcebdd3c-06b2-49dd-bb13-6db0d6bc3dc1)

### Return
The Python return statement is a special statement inside a function or method to send the function’s result back to the caller. 
- A return statement consists of the return keyword followed by an optional return value.
- functions can return numeric values (int, float, and complex values), collections and sequences of objects (list, tuple, dictionary, or set objects), user-defined objects, classes, functions, and even modules or packages.

![Screenshot (772)](https://github.com/Rnovranza/Python_Week_2/assets/134476980/b01fd54d-adc1-491c-a001-8ecfe0464091)

A function's output can be saved in a variable, setting it apart from a void function that doesn't produce any output. This distinctive characteristic determines if a value is provided by the function.

![Screenshot (775)](https://github.com/Rnovranza/Python_Week_2/assets/134476980/5cd1747d-cd1e-4b2d-9f4c-7b365f28012d)

### Pass by reference vs value
- all parameters (arguments) in python are pass by reference vs value meaning that when we change a var then the data that refers to it will also change, both within the function and outside the function.
- except when performing assignment operations that will change the parameter reference

#### - Pass by value
The value of the variable is copied and passed to the function. Changes to parameters inside the function do not affect the original variables outside the function.

![Screenshot (777)](https://github.com/Rnovranza/Python_Week_2/assets/134476980/ae1c3ab3-7653-47ff-b063-0486b7b6ffdc)
In the above example, although the value of r is changed inside the function, the value of radius outside the function remains unchanged.

#### - Pass by reference
The memory address of the variable is passed to the function. Changes to the parameters inside the function will affect the original variables outside the function.

![Screenshot (779)](https://github.com/Rnovranza/Python_Week_2/assets/134476980/cf43493b-a384-44ab-9509-beb97fb47902)
###### 
Since we only appended a value to the list without reassigning the variable, there is no decoupling or recoupling taking place. Both the inner and outer variables still refer to the same object, while the content of that object has been altered by the addition of the new value.

## Numpy
NumPy is a Python library that provides multidimensional array objects, various derived objects (such as masked arrays and matrices), and various routines for fast operations on arrays, including math, logic, shape manipulation, sorting, selection, I/O, discrete Fourier transform, basic linear algebra, basic statistical operations, random simulation, and more.

NumPy usually imported under the np alias.

![Screen Shot 2024-04-20 at 05 53 23](https://github.com/Rnovranza/Python_Week_2/assets/121234567/0a378ea5-28ad-4fad-80ea-b89dfa9609aa)

The fundamental object in NumPy is the ndarray (n-dimensional array). You can create ndarray objects using the array() function, passing in sequences like lists or tuples. This allows for efficient storage and manipulation of large data sets, making NumPy an essential tool for scientific computing and data analysis in Python.

![Screen Shot 2024-04-20 at 05 40 11](https://github.com/Rnovranza/Python_Week_2/assets/121234567/0c5302df-3eca-437d-9f24-d94fc74958ab)

The array() method in NumPy is quite flexible in what it can accept. You can pass in Python lists, tuples, or any other array-like object, and it will convert it into a NumPy ndarray. This flexibility makes it convenient to work with various data structures and seamlessly integrate them into your numerical computations using NumPy.

![Screen Shot 2024-04-20 at 05 40 28](https://github.com/Rnovranza/Python_Week_2/assets/121234567/40e949b2-2b5e-476c-99f4-f749c4d73a2f)

### Dimension In Arrays
A dimension in an array refers to one level of nested arrays within it. There are several dimensions that we can recognize as follows:  

#### 1. 0-D Arrays
Scalars, also known as 0-D arrays, represent individual elements within an array structure. In essence, every value contained within an array constitutes a 0-D array.

![Screen Shot 2024-04-20 at 05 42 22](https://github.com/Rnovranza/Python_Week_2/assets/121234567/c2b0f586-ed3c-4e17-a563-ee5b52864cb3)

#### 2. 1-D Arrays
A uni-dimensional or 1-D array typically consists of a single sequence of elements and is considered one of the most fundamental and commonly used array structures.

![Screen Shot 2024-04-20 at 05 42 30](https://github.com/Rnovranza/Python_Week_2/assets/121234567/ccca583f-0fe6-41f4-b14a-62ca552c0659)

#### 3. 2-D Arrays
A 2-D array, also known as a two-dimensional array, consists of arrays (or lists) as its elements, each of which is itself a one-dimensional array. This structure is commonly used to represent matrices or 2nd order tensors.

![Screen Shot 2024-04-20 at 06 46 37](https://github.com/Rnovranza/Python_Week_2/assets/121234567/4b5a6a5b-d480-44c7-b2b0-52a62cc7c3b8)

#### 3. 3-D Arrays
A 3-D array, also known as a three-dimensional array, comprises matrices (or 2-D arrays) as its elements. These arrays are commonly utilized to represent a 3rd order tensor.

![Screen Shot 2024-04-20 at 05 42 42](https://github.com/Rnovranza/Python_Week_2/assets/121234567/650ca7df-2438-487d-b859-cf60714d28ae)

In NumPy, the ndim attribute is used to determine the number of dimensions (or axes) of a NumPy array. It returns an integer value indicating the number of dimensions present in the array. This attribute is useful for understanding the structure of the array and for performing conditional operations based on the array's dimensionality.

![Screen Shot 2024-04-20 at 05 42 55](https://github.com/Rnovranza/Python_Week_2/assets/121234567/9e334398-f53a-4f14-b2ef-1b1aae652211)

Indexing an array in NumPy works similar to how you access elements in a Python list. You refer to a particular element in an array by specifying its index number. In NumPy, as in Python, indexing starts from 0, so the first element of the array has index 0, the second element has index 1, and so on. This convention makes it consistent with other programming languages and eases the manipulation of array elements. An example is as follows:

![Screen Shot 2024-04-20 at 05 43 25](https://github.com/Rnovranza/Python_Week_2/assets/121234567/c6cdeadf-cc9e-463f-9df0-5f1b748e85ea)

When working with 2-D arrays, you can use comma-separated integers within square brackets to specify both the row and column indices of the element you want to access. This notation resembles the way you'd reference cells in a table, where one index represents the row (dimension) and the other represents the column (index). This intuitive indexing scheme makes it easy to interact with the data stored in 2-D arrays, as you can directly address individual elements based on their row and column positions.

![Screen Shot 2024-04-20 at 05 45 05](https://github.com/Rnovranza/Python_Week_2/assets/121234567/a5965308-f261-4b97-bae9-242d9ebfbfc2)

When dealing with 3-D arrays, you extend the comma-separated indexing approach to include three integers inside square brackets. These integers represent the index along each dimension of the array. So, just like a 2-D array, you can think of a 3-D array as a stack of 2-D arrays (or matrices). Each integer specifies the index of an element along the respective dimension, allowing you to specify a particular element in the array. 

![Screen Shot 2024-04-20 at 05 45 19](https://github.com/Rnovranza/Python_Week_2/assets/121234567/61aa07b7-99cb-481e-aa49-542a7dd109a2)

Negative indexing in NumPy allows you to access elements of an array relative to the end of the array. For instance, if you want to access the last element of an array, you can use an index of -1. Similarly, -2 refers to the second-to-last element, and so on. This is particularly useful when you need to access elements near the end of the array and you don't know the exact length of the array. Here's an example:

![Screen Shot 2024-04-20 at 07 04 55](https://github.com/Rnovranza/Python_Week_2/assets/121234567/7c47168d-955f-4916-a30f-60783fc63903)

## Pandas

### Data Series
data series is a one-dimensional labeled array you can use to work with data. It's part of the powerful pandas library commonly used for data analysis in Python.

![Screenshot 2024-04-20 103923](https://github.com/Rnovranza/Python_Week_2/assets/101807673/3cab6081-8dc5-4840-96a4-c874544df348)

#### Implicit and Explicit Indexing
Indexing refers to how you label and retrieve data elements. There are two main types of indexing: implicit and explicit.

Implicit Index:
- Relies on the positional order of data within the series.
- Similar to how you access elements in Python lists using numerical indexes (0, 1, 2, etc.).
- Starts from 0 (zero-based indexing).

Explicit Index:
- Uses custom labels assigned to each data point.
- Offers more meaningful and descriptive way to access data.
- You can set a column or another series as the index.

![Screenshot 2024-04-20 104037](https://github.com/Rnovranza/Python_Week_2/assets/101807673/9d55508d-4a08-4f32-92ea-e691155b70eb)

#### Data Slicing in Data Series
Data slicing in a data series (part of the pandas library) in Jupyter notebooks allows you to extract specific subsets of data based on certain criteria. It's a powerful tool for manipulating and analyzing your data.

![Screenshot 2024-04-20 104133](https://github.com/Rnovranza/Python_Week_2/assets/101807673/4d82a0d0-cb54-4f0e-9bc8-a2bda40df286)

#### .loc and .iloc
.loc and .iloc are essential methods for selecting data by label and position in pandas DataFrames (relational data structures) within Jupyter notebooks. They provide powerful and flexible ways to access and manipulate specific rows and columns.
 .loc:
Primarily used for selecting data by labels (explicit indexing) assigned to the data series. Use .loc when your labels are meaningful and descriptive for better code readability.

 .iloc:
Works with the integer positions (implicit indexing) of elements within the series. might be slightly faster for operations based on integer positions, especially for large datasets. However, the performance difference is often negligible for most use cases.

![Screenshot 2024-04-20 104218](https://github.com/Rnovranza/Python_Week_2/assets/101807673/990ec0ac-bd0c-4f95-917b-dd55c9c8e8b5)

#### Dictionary
A dictionary is a powerful way to provide initial data for a data series. Each key-value pair in the dictionary becomes a label-value pair in the series.

![Screenshot 2024-04-20 104255](https://github.com/Rnovranza/Python_Week_2/assets/101807673/78a7e64d-0a96-47ba-8213-478970042aae)


### Data Frame
DataFrame in pandas is a fundamental data structure specifically designed for data analysis and manipulation in Python. It essentially acts as a powerful spreadsheet on steroids but with the added benefits of programming logic and automation. A DataFrame is indeed a collection of Series, where each Series represents a single column of data.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165742717/467ba473-e5a8-4809-8ec6-67c13e3977bd)


In the realm of data analysis using Python's pandas library, converting a CSV (Comma-Separated Values) file into a pandas DataFrame is a fundamental step.
The operations that can be used on CSV data loaded into a DataFrame are as follows :

#### 1.	Reading and Loading CSV Data

Use the pd.read_csv() function to read data from a CSV file into a DataFrame.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165742717/e7c8665d-22a5-4fd8-8553-b2e0637702c4)

Once you have your DataFrame loaded, you can use various methods to explore its content:

-	df.head(): View the first 5 rows by default.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165742717/700cdeff-0f1d-4aab-91b9-a9101e0e2b05)

-	df.tail(): View the last 5 rows by default.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165742717/0fcadcdb-5da5-469e-a660-69329eeea4a9)


-	df.info(): Get summary information about the DataFrame (data types, non-null values, etc.).

![image](https://github.com/Rnovranza/Python_Week_2/assets/165742717/d1e52720-5c70-4301-b846-76b6e0da9115)


-	df.shape: returns a tuple containing two integers representing the dimensions of the DataFrame.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165742717/f63e983e-b29a-49dc-8790-ef19c25e3c1d)


-	df.columns: retrieves an Index object containing the labels for each column in the DataFrame.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165742717/bb333f24-9350-4b7f-b0a2-9f731130e5d0)

-	df.index: returns the Index object associated with the rows of the DataFrame.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165742717/ff0cfaf9-5193-47ea-a976-46a0e96b333f)


#### 2.	Descriptive Statistics
Descriptive statistics focus on numerical columns within your DataFrame. They provide a concise overview of the data distribution. 
The describe() method in pandas is the primary tool for generating descriptive statistics for numerical columns in a DataFrame.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165742717/ad9ee9e5-4f56-43c3-938b-da57b32804c8)



#### 3.	Data Aggregation
Data aggregation involves combining or grouping data points based on a specific criterion and applying a function to calculate a single value for the group.
Common Aggregation Functions:

-	mean(): Computes the average value in a column or group.

-	median(): Determines the middle value in a sorted list of values within a column or group (useful for skewed data).

-	mode(): The most frequent value in the data.

-	min(): Finds the minimum value in a column or group.

-	max(): Identifies the maximum value in a column or group.


![image](https://github.com/Rnovranza/Python_Week_2/assets/165742717/51d5a2ea-7546-4cae-8394-e21ca8e1a195)



#### 4.	Finding and Counting Distinct Values
Finding and counting distinct values refers to the process of identifying and calculating the number of unique elements within a dataset, typically focusing on a single column in a pandas DataFrame.

-	unique(): This function is used to identify and return all the distinct values (unique elements) present in a specific column.

-	nunique(): This is a pandas-specific function that directly calculates the number of unique values (distinct elements) within a DataFrame column.


![image](https://github.com/Rnovranza/Python_Week_2/assets/165742717/d0dec0ee-93af-4ab0-8dd7-86d5e3e7348c)



It can look at the proportion of the Gender column or count the number of unique values in the "Gender" column of the DataFrame (called df). The result will return a Pandas Series containing the number of occurrences of each unique value, with the value as the index and the number of occurrences as the value in the Series. This gives a good understanding of the distribution of values in the "Gender" column of the DataFrame.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/32ee872d-255e-41f9-b7c1-bc89b47f490e)

Can select specific columns from a DataFrame. The result will be a new DataFrame containing only the selected columns. By using this syntax, it is easier to select a specific subset of DataFrame columns that match the needs of data analysis or processing.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/b6292164-b22d-486a-a3fb-4f7ad1b9ea9f)

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/50d04578-19d5-4d89-8f7c-cd30d3fbb7e6)

In Python, when you want to create conditions or criteria in your code, you can use comparison operators and logical operators. Here is a brief explanation of these operators:

1. Comparison Operators:
- `>` (more than): This operator is used to check if the value on the left is greater than the value on the right.
- `<` (less than): This operator is used to check if the value on the left is less than the value on the right.
- `>=` (greater than or equal to): This operator is used to check if the value on the left is greater than or equal to the value on the right.
- `<=` (less than or equal to): This operator is used to check if the value on the left is less than or equal to the value on the right.
- `==` (equal to): This operator is used to check if the value on the left is equal to the value on the right.
- `!=` (not equal to): This operator is used to check if the value on the left is not equal to the value on the right.

2. Logical Operators:
- `and`: This operator returns True if both compared conditions are true.
- `or`: This operator returns True if one or both of the compared conditions are true.
- `not`: This operator is used to reverse the truth value of a condition.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/87212435-b4ec-4459-84a5-7c298c965409)

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/a3897cc2-4d5d-4561-8233-c6165b03de1c)

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/04536fc9-d980-4ec7-8924-3ff2058ec2ea)

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/39d8dfdd-b962-4514-b809-075c445aa793)

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/3b52c309-e630-4f72-9365-fb6d25909953)

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/93c0d87d-c45c-45b7-905f-5d9c3b3b8b36)

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/0f85f7e7-9f46-4f06-b2de-66e7e6774b80)

## Random Library
The random library in Python is a built-in module that provides various functions to perform random operations. It is used to generate random numbers, randomly select items from a list, and randomize the order of elements in a list or array

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/106ee879-5fd3-413a-a616-d82cb799cb39)

## Datetime Library
The datetime module can be used to work with dates and times, including
1. Creating random dates and times
2. Creating a Random Time within a Specified Time Range
3. Combining Date and Time

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/f25a972d-3965-45c2-9f41-4d61771ea56c)

Then the format can also be changed according to your needs.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/5a082ace-aad6-407d-a035-2689b4e0ded2)

## txt file - open, read, close
Importing text files into Python is a commonly used process in data analysis, text processing, and many other applications. In Python, you can open, read, and close text files using some built-in functions (with a .txt extension).

`Open`
Open a text file using the open() function and need to provide the file name and access mode. The r access mode is used to read the file.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/6ce5e1d7-eb36-437e-b7d2-e5196f792adc)

`Read`
After opening the file, it can read its contents using the read() method or other methods such as readline() to read line by line.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/dcc83741-260c-4e50-8565-75b9b6d50070)

`Close`
After finishing reading or performing other operations on a file, it is important to close it using the close() method.

![image](https://github.com/Rnovranza/Python_Week_2/assets/165861920/26151079-60da-4fe1-9a8d-0f04aee076fe)











