# Experiment 12: Categorical Data Analysis Using Python

## Aim

To study and perform **categorical data analysis using Python (Pandas library)**, including frequency distribution, percentage analysis, cross-tabulation, grouping, filtering, and sorting of categorical variables.

---
## Note: This experiment contains a dataset uploaded seperately for the purpose. It can be found within the repository itself with the name: Exp12_data.csv. If there are some issues with that file, the data used for dataset 1 is uploaded for reference at the end of this readme just in case. 
## Theory

**Categorical Data Analysis** involves analyzing data that can be divided into distinct groups or categories. These categories may or may not have an inherent order.

### Types of Categorical Data

1. **Nominal Data**
   - Categories without any order  
   - Examples: Gender, Department, Blood Group  

2. **Ordinal Data**
   - Categories with a meaningful order or ranking  
   - Examples: Grades (A, B, C), Ratings (Good, Better, Best), Education Level  

---

## Dataset 1: Student Data Analysis

The dataset is loaded using:

```python
import pandas as pd
df = pd.read_csv("Expt11.csv")
````

This dataset contains categorical variables such as:

* Gender
* Department
* Grade

---

### 1. Frequency Distribution

```python
df['Grade'].value_counts()
```

* Counts the number of occurrences of each category
* Helps understand how data is distributed

---

### 2. Department-wise Count

```python
df['Department'].value_counts()
```

* Provides number of students in each department

---

### 3. Percentage Distribution

```python
df['Grade'].value_counts(normalize=True) * 100
```

* Converts frequency into percentage
* `normalize=True` gives proportion
* Multiplying by 100 converts it to percentage

---

### 4. Gender Count

```python
df['Gender'].value_counts()
```

* Counts number of males and females

---

### 5. Cross Tabulation (Contingency Table)

```python
pd.crosstab(df['Gender'], df['Grade'])
```

* Shows relationship between two categorical variables
* Example: Gender vs Grade distribution

---

### 6. Department vs Gender

```python
pd.crosstab(df['Department'], df['Gender'])
```

* Helps analyze gender distribution across departments

---

### 7. Department vs Grade

```python
pd.crosstab(df['Department'], df['Grade'])
```

* Shows grade distribution across departments

---

### 8. Percentage Crosstab (Normalization)

```python
pd.crosstab(df['Department'], df['Grade'], normalize='index') * 100
```

* Converts counts into percentages row-wise

#### Normalization Types:

* `normalize=True` or `'all'`
  → Entire table normalized

* `normalize='index'`
  → Row-wise normalization

* `normalize='columns'`
  → Column-wise normalization

---

### 9. Grouping Data

```python
df.groupby('Department')['Grade'].value_counts()
```

* Groups data by department
* Then counts grades within each group
* Useful for hierarchical analysis

---

## Dataset 2: E-Commerce Data Analysis

A dataset is created using dictionary:

```python
data = {
    'Order_ID':['O1','O2','O3','O4','O5','O6','O7','O8','O9','O10'],
    'Category':['Electronics','Clothing','Electronics','Grocery','Clothing',
                'Electronics','Grocery','Clothing','Electronics','Grocery'],
    'Payment_Method':['UPI','Card','UPI','Cash','Card',
                      'UPI','Cash','Card','UPI','Cash'],
    'Delivery_Type':['Express','Standard','Express','Standard','Express',
                     'Standard','Express','Standard','Express','Standard'],
    'Customer_Type':['New','Returning','Returning','New','Returning',
                     'New','Returning','New','Returning','New']
}

df = pd.DataFrame(data)
```

---

### 1. Category Frequency

```python
df['Category'].value_counts()
```

* Counts number of orders per category

---

### 2. Payment Method Frequency

```python
df['Payment_Method'].value_counts()
```

* Shows most commonly used payment methods

---

### 3. Percentage Distribution

```python
df['Payment_Method'].value_counts(normalize=True) * 100
```

* Shows percentage usage of each payment method

---

### 4. Filtering Data

```python
df[df['Category'] == 'Electronics']
```

* Filters dataset based on condition
* Returns only electronics orders

---

### 5. Sorting Data

```python
df.sort_values(by='Category')
```

* Sorts dataset based on column values

---

### 6. Unique Values

```python
df['Category'].unique()
```

* Returns all unique categories

---

### 7. Number of Unique Values

```python
df['Category'].nunique()
```

* Returns count of distinct categories

---

### 8. Crosstab (Category vs Payment Method)

```python
pd.crosstab(df['Category'], df['Payment_Method'])
```

* Shows relationship between category and payment method

---

### 9. Grouping Multiple Columns

```python
df.groupby(['Category','Payment_Method']).value_counts()
```

* Groups data based on multiple columns
* Provides detailed frequency distribution

---

## Key Concepts Covered

* Categorical data types (Nominal & Ordinal)
* Frequency distribution using `value_counts()`
* Percentage analysis using `normalize=True`
* Cross-tabulation using `pd.crosstab()`
* Data grouping using `groupby()`
* Filtering using conditions
* Sorting using `sort_values()`
* Unique value analysis using `unique()` and `nunique()`

---

## Conclusion

In this experiment, categorical data analysis was performed using the **Pandas library**.

The experiment helped in:

* Understanding different types of categorical data
* Performing frequency and percentage analysis
* Analyzing relationships using cross-tabulation
* Applying grouping and filtering techniques
* Extracting meaningful insights from categorical datasets

Thus, categorical data analysis is an essential technique in **data science, business analytics, and decision-making processes**.

---
# Dataset 1 for reference: 
<img width="321" height="645" alt="dataset 1_image1" src="https://github.com/user-attachments/assets/6d64b2f0-7d19-4e56-b849-5e8a4dfeb6e9" />
<img width="298" height="542" alt="dataset 1_image2" src="https://github.com/user-attachments/assets/81ddc0a7-7e4f-42fc-abea-4bd9fa9cfd26" />

---
## 👨‍💻 Author

**Rachit Jajoo**
Electronics & Telecommunication Engineering (ENTC)
Symbiosis Institute of Technology, Pune
