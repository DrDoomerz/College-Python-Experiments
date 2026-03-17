# 🧪 Experiment 10 – Study of Pandas Library

---

## 🎯 Aim

To study the Pandas library in Python and understand how to create, manipulate, analyze, and filter structured data using Series and DataFrames.

---

## 📚 Theory

### 🔹 Introduction to Pandas

Pandas (Panel Data) is a powerful Python library used for:

* Handling structured and tabular data
* Data manipulation and preprocessing
* Statistical analysis
* Data filtering and transformation

It provides two main data structures:

* **Series** → One-dimensional labeled array
* **DataFrame** → Two-dimensional labeled data structure (tabular format)

---

# 🔍 Commands Used in the Experiment

## 1️⃣ Importing Pandas

```python
import pandas as pd
```

* Imports the Pandas library.
* `pd` is an alias used to access Pandas functions.

---

## 2️⃣ Creating a Series

```python
s = pd.Series([10,20,30,40])
```

### `pd.Series()`

* Creates a one-dimensional labeled array.
* Automatically assigns index values starting from 0.
* Stores values along with datatype information.

---

## 3️⃣ Creating a DataFrame

```python
data = {
 "Name":["A","B","C"],
 "Marks":[85,90,78]
}

DF = pd.DataFrame(data)
```

### `pd.DataFrame()`

* Creates a two-dimensional tabular structure.
* Dictionary keys become column names.
* Values become column data.

---

## 📌 DataFrame Commands (As Per Experiment)

## 🔹 Command 1 – `DF.shape`

```python
DF.shape
```

* Returns tuple `(rows, columns)`.
* Example: `(3,2)` means 3 rows and 2 columns.

---

## 🔹 Command 2 – `DF.ndim`

```python
DF.ndim
```

* Returns number of dimensions.
* A DataFrame is always 2-dimensional.

---

## 🔹 Command 3 – `DF.size`

```python
DF.size
```

* Returns total number of elements.
* Calculated as rows × columns.

---

## 🔹 Command 4 – `DF.columns`

```python
DF.columns
```

* Returns list of column names.
* Output type: Index object.

---

## 🔹 Command 5 – `DF.dtypes`

```python
DF.dtypes
```

* Returns datatype of each column.
* Example:

  * Name → object
  * Marks → int64

---

## 🔹 Command 6 – Accessing a Column

```python
DF["Name"]
```

* Returns the entire "Name" column.
* Output type → Series.

---

## 🔹 Command 7 – Accessing Data Using `loc`

```python
DF.loc[0,"Name"]
```

* Label-based indexing.
* Syntax: `df.loc[row_label, column_label]`
* Used to access specific row and column by label.

---

## 🔹 Command 8 – Accessing Data Using `iloc`

```python
DF.iloc[2,1]
```

* Position-based indexing.
* Syntax: `df.iloc[row_index, column_index]`
* Used to access data by integer position.

---

## 🔹 Command 9 – Adding a New Column

```python
DF["Grade"] = ["First Class", "Distinction", "Second Class"]
```

* Adds a new column to the DataFrame.
* Length must match number of rows.

---

## 🔹 Command 10 – `DF.drop()`

### Creating a New DataFrame Without Column

```python
DF1 = DF.drop("Grade", axis=1)
```

* Removes specified column.
* `axis=1` refers to column.
* Returns new DataFrame.

### Dropping Column In-Place

```python
DF.drop("Grade", axis=1, inplace=True)
```

* Permanently deletes column.
* `inplace=True` modifies original DataFrame.

---

## 🔹 Command 11 – `mean()`

```python
DF["Marks"].mean()
```

* Calculates average value of the column.
* Used for statistical analysis.

---

## 🔹 Command 12 – `min()`

```python
DF["Marks"].min()
```

* Returns minimum value in the column.
* Identifies lowest value.

---

## 🔹 Command 13 – `max()`

```python
DF["Marks"].max()
```

* Returns maximum value in the column.
* Identifies highest value.

---

## 🔹 Filtering (Boolean Indexing)

```python
DF[DF["Marks"] > 80]
```

* Filters rows based on condition.
* Returns only rows where marks are greater than 80.
* This is called Boolean Indexing.

---

# 📊 Observations

* Pandas efficiently handles structured and tabular data.
* Series is suitable for single-column data.
* DataFrame is ideal for multi-column datasets.
* `loc` and `iloc` allow flexible data access.
* Columns can be added, modified, and removed easily.
* Built-in statistical functions simplify analysis.
* Filtering helps extract meaningful subsets of data.

---

# Conclusion

The experiment successfully demonstrated the use of the Pandas library for handling structured data using Series and DataFrames.

Various operations such as creating data structures, accessing elements, modifying values, deleting columns, performing statistical calculations, and filtering data were performed successfully. Pandas provides a powerful, flexible, and efficient framework for data analysis in engineering and data science applications.

---

## 👨‍🎓 Student Details

* **Name:** Rachit Jajoo
* **PRN:** 25070123088
* **Branch:** Electronics and Telecommunication (ENTC)
* **Batch:** B1
* **Institute:** Symbiosis Institute of Technology, Pune
