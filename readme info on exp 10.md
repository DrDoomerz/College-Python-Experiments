# Experiment 10: Study of Pandas Library

## Aim

To study the **Pandas library in Python** and perform operations such as creating Series and DataFrames, accessing data, modifying data, deleting columns, and performing basic statistical analysis and filtering.

---

## Theory

**Pandas** (Panel Data) is a powerful open-source Python library used for **data manipulation and analysis**. It provides efficient and flexible data structures to handle structured data.

The two primary data structures in Pandas are:

### 1. Series

A **Series** is a one-dimensional labeled array capable of holding data of any type (integers, strings, floats, etc.).

Example:
```python
import pandas as pd
s = pd.Series([10,20,30,40])
````

---

### 2. DataFrame

A **DataFrame** is a two-dimensional data structure (like a table) consisting of rows and columns.

Example:

```python
data = {
    "Name":["A","B","C"],
    "Marks":[85,90,78]
}
DF = pd.DataFrame(data)
```

---

## Important Pandas Concepts

### 1. Viewing Data

* `df.head()` → Displays first 5 rows
* `df.tail()` → Displays last 5 rows

---

### 2. Understanding Data Structure

* `df.shape` → Returns number of rows and columns
* `df.ndim` → Returns dimension
* `df.size` → Returns total number of elements
* `df.columns` → Returns column names
* `df.dtypes` → Shows datatype of each column

---

### 3. Accessing Data

* `df["column"]` → Access entire column
* `df.loc[row, column]` → Label-based access
* `df.iloc[row, column]` → Index-based access

---

### 4. Modifying Data

* Add new column:

```python
DF["Grade"] = ["First Class", "Distinction", "Second Class"]
```

* Update values using:

  * `loc[]`
  * `iloc[]`

---

### 5. Deleting Data

* `df.drop(column, axis=1)` → Removes column
* `inplace=True` → Applies changes to original DataFrame

---

### 6. Statistical Operations

* `df.mean()` → Average
* `df.min()` → Minimum
* `df.max()` → Maximum

---

### 7. Filtering Data

Used to extract rows based on conditions:

```python
DF[DF["Marks"] > 80]
```

---

## Algorithms

---

### 🔹 Algorithm 1: Creating a Series

1. Start the program.
2. Import the Pandas library.
3. Create a list of elements.
4. Convert the list into a Series using `pd.Series()`.
5. Display the Series.
6. End the program.

---

### 🔹 Algorithm 2: Creating a DataFrame

1. Start the program.
2. Import Pandas library.
3. Create a dictionary containing column names and values.
4. Convert dictionary into DataFrame using `pd.DataFrame()`.
5. Display the DataFrame.
6. End the program.

---

### 🔹 Algorithm 3: Finding Structure of DataFrame

1. Start the program.
2. Create a DataFrame.
3. Use `df.shape` to find rows and columns.
4. Use `df.ndim` to find dimensions.
5. Use `df.size` to find total elements.
6. Use `df.columns` to display column names.
7. Use `df.dtypes` to display data types.
8. Display all outputs.
9. End the program.

---

### 🔹 Algorithm 4: Accessing Data

1. Start the program.
2. Create a DataFrame.
3. Access a column using `df["column_name"]`.
4. Access specific element using `df.loc[row, column]`.
5. Access element using index with `df.iloc[row, column]`.
6. Display the results.
7. End the program.

---

### 🔹 Algorithm 5: Adding a New Column

1. Start the program.
2. Create a DataFrame.
3. Define a new column with values.
4. Add the column using `df["new_column"] = values`.
5. Display updated DataFrame.
6. End the program.

---

### 🔹 Algorithm 6: Updating Data in DataFrame

1. Start the program.
2. Create a DataFrame.
3. Identify the value to be updated.
4. Use `df.loc[row, column] = new_value` to update.
5. Alternatively, use `df.iloc[row_index, column_index] = new_value`.
6. Display updated DataFrame.
7. End the program.

---

### 🔹 Algorithm 7: Deleting a Column

1. Start the program.
2. Create a DataFrame.
3. Identify the column to be deleted.
4. Use `df.drop("column_name", axis=1)` to remove column (new DataFrame).
5. Use `inplace=True` to modify original DataFrame.
6. Display updated DataFrame.
7. End the program.

---

### 🔹 Algorithm 8: Performing Statistical Analysis

1. Start the program.
2. Create a DataFrame.
3. Select numerical column.
4. Use `mean()` to calculate average.
5. Use `min()` to find minimum value.
6. Use `max()` to find maximum value.
7. Display all results.
8. End the program.

---

### 🔹 Algorithm 9: Filtering Data

1. Start the program.
2. Create a DataFrame.
3. Apply condition using comparison operator (e.g., Marks > 80).
4. Use DataFrame filtering syntax `df[condition]`.
5. Display filtered data.
6. End the program.

---

## Conclusion

In this experiment, the **Pandas library** was studied and implemented for handling structured data .

The experiment helped in:

* Understanding Series and DataFrame structures
* Performing data access and modification
* Learning column operations (add, update, delete)
* Applying statistical functions
* Filtering data efficiently

Thus, Pandas is a **powerful tool for data analysis** and widely used in real-world applications such as data science, machine learning, and analytics.

---

## 👨‍💻 Author

**Rachit Jajoo**
Electronics & Telecommunication Engineering (ENTC)
Symbiosis Institute of Technology, Pune
