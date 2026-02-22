# STUDY-OF-PANDAS-IN-PYTHON





#  EXPERIMENT NO: 9

# TITLE: Study of Pandas

**Name:** Amey Waghmare
**PRN:** 25070123009
**Batch:** A1

---

#  AIM

To study and implement the basic operations of Pandas library including Series creation, DataFrame creation, data manipulation, data cleaning, and statistical analysis.



#  THEORY 

##  Introduction to Pandas

pandas is an open-source Python library used for handling structured data. It is mainly used for:

* Data cleaning
* Data manipulation
* Data analysis
* Handling missing data
* Working with CSV, Excel, SQL files

Pandas is built on top of NumPy and is widely used in **Data Science, Machine Learning, and Exploratory Data Analysis (EDA).**


##  Why Pandas is Important?

In real-world applications, data is usually:

* Structured (rows and columns)
* Stored in tables
* Large in size
* Containing missing or inconsistent values

Pandas provides powerful tools to:

* Organize data
* Modify data
* Filter data
* Perform statistical analysis efficiently



#  Core Data Structures in Pandas

Pandas mainly provides two important data structures:

---

## 1️ Series

A **Series** is a one-dimensional labeled array.

It:

* Stores data in a single column
* Has an index
* Can hold different data types

Example:

python
import pandas as pd

s = pd.Series([7,8,10,18,45])


Here:

* Values are stored
* Index is automatically assigned (0,1,2,3...)



## 2️ DataFrame

A **DataFrame** is a two-dimensional labeled data structure (like a table).

It:

* Has rows and columns
* Each column can have different data types
* Is similar to Excel sheet or SQL table

Example:

python
data = {
    "Name":["A","B","C","D"],
    "Marks":[85,90,95,100]
}
df = pd.DataFrame(data)




#  Important DataFrame Operations

---
##  Viewing Data

### `head()`

Displays first 5 rows.

python
df.head()


### `tail()`

Displays last 5 rows.

python
df.tail()



##  Structure of DataFrame

### `shape`

Returns (rows, columns)

python
df.shape


### `ndim`

Returns number of dimensions.

python
df.ndim


### `size`

Returns total number of elements.

python
df.size




##  Column Information

### `columns`

Displays column names.

python
df.columns


### `dtypes`

Shows data type of each column.

python
df.dtypes



## Accessing Data

### Access Column

python
df["Name"]


### Access Row (Using loc)

python
df.loc[1]



##  Modifying Data

### Adding New Column

`python
df["Grade"] = ["First Class","Distinction","Second Class","Fail"]


### Updating Data

python
df.loc[0,"Marks"] = 88


### Dropping Column

python
df.drop("Grade", axis=1, inplace=True)




#  Statistical Operations

Pandas provides built-in statistical functions:

### Mean

python
df["Marks"].mean()


### Maximum

python
df["Marks"].max()


### Minimum

```python
df["Marks"].min()
```

These functions are very useful in:

* Data summarization
* Academic result analysis
* Business analytics

---

#  Conditional Filtering

Pandas allows filtering based on conditions.

Example:

```python
df[df["Marks"] > 90]
```

This returns only rows where Marks are greater than 90.

Conditional filtering is important for:

* Selecting top performers
* Removing unwanted records
* Data segmentation

---

#  SYNTAX

##  Import Pandas

```python
import pandas as pd
```

---

##  Create Series

```python
pd.Series(data)
```

---

##  Create DataFrame

```python
pd.DataFrame(dictionary)
```

---

##  View Data

```python
df.head()
df.tail()
```

---

##  Structure Information

```python
df.shape
df.ndim
df.size
df.columns
df.dtypes
```

---

##  Access Data

```python
df["column_name"]
df.loc[row_index]
```

---

##  Modify Data

```python
df["new_column"] = values
df.loc[row_index,"column"] = new_value
df.drop("column_name", axis=1, inplace=True)
```

---

##  Statistical Functions

```python
df["column"].mean()
df["column"].max()
df["column"].min()
```

---

##  Conditional Filtering

```python
df[df["column"] > value]
```

---

#  CONCLUSION

In this experiment, the Pandas library was studied and implemented successfully.

We learned:

* Creation of Series and DataFrame
* Viewing and analyzing structured data
* Accessing and modifying data
* Performing statistical operations
* Applying conditional filtering

This experiment helped in understanding how structured data is handled efficiently using Pandas, which is an essential tool in Data Science and Data Analysis.

---


