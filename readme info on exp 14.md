
# Experiment 14: Data Binning and Data Formatting in Python

---

## 🎯 Aim
To perform data binning and data formatting on datasets using Python and understand how continuous data can be converted into meaningful categorical information.

---

## 📚 Theory

### 🔹 1. Introduction to Data Binning

Data binning (also known as discretization) is the process of converting continuous numerical data into discrete categories or groups (bins). This is particularly useful when raw numerical values are difficult to interpret directly.

Instead of analyzing raw values (like price or delivery time), binning allows us to:

* Group data into meaningful ranges
* Identify patterns more easily
* Reduce noise in data
* Simplify analysis and visualization

For example, instead of using exact prices, products can be classified as:

* Low
* Medium
* High

This improves interpretability without losing essential trends.

---

### 🔹 2. Concept of Bins and Labels

Binning is performed using:

* **Bins:** Numerical intervals defining ranges
* **Labels:** Names assigned to each interval

Using `pd.cut()`:

* Values are placed into intervals
* Each interval is assigned a label
* Output becomes a **categorical variable**

As observed in Dataset 1, prices were divided into:

* 0–10000 → Low
* 10000–30000 → Medium
* 30000–60000 → High

---

### 🔹 3. Data Binning in Practice

#### 📌 Dataset 1: Product Data

This dataset includes:

* Product name
* Price
* Units sold

Binning was applied to:

##### Price Categorization

* Converts continuous price into categories
* Helps identify product pricing tiers

High-priced products like laptops and cameras fall into the “High” category, while accessories fall into “Low”.

##### Sales Categorization

* Units sold were grouped into:

  * Low Sales
  * Medium Sales
  * High Sales

Even low-priced items (like headphones) show high sales, indicating that demand is not directly dependent on price.

---

#### 📌 Dataset 2: Food Delivery Data

This dataset includes:

* Order value
* Delivery time
* Distance

Binning was applied to multiple features:

##### Order Value Categorization

* Classifies order size into Low, Medium, High

##### Delivery Speed Categorization

* Based on delivery time:

  * Fast
  * Medium
  * Slow

##### Distance Categorization

* Groups distances into:

  * Short
  * Medium
  * Long

Shorter distances generally correspond to faster deliveries, while longer distances tend to align with slower delivery speeds, showing a practical relationship between variables.

---

### 🔹 4. Data Types and Categorical Conversion

After binning, columns are converted into **categorical data types**.

Advantages:

* Reduced memory usage
* Better performance
* Efficient category-based analysis

---

### 🔹 5. Data Formatting

Data formatting ensures consistency and correctness in the dataset.

#### Data Type Conversion

* Integer values were converted to float where required to allow flexible numerical operations

#### Text Standardization

* Text values were converted to uppercase to maintain uniformity and avoid duplication

#### Rounding Values

* Numerical values were rounded for consistency and readability

---

### 🔹 6. Sorting and Data Organization

Sorting improves readability and helps identify trends.

* Products were sorted based on price (descending)
* Orders were sorted based on order value (ascending)

This makes comparison and analysis more structured.

---

### 🔹 7. Frequency Analysis

Frequency distribution helps understand how data is spread across categories.

* Most deliveries fall under the **Fast** category
* Distance distribution is concentrated in Medium and Long ranges
* Order categories are relatively balanced

---

## ⚙️ Commands Used & Explanation

### Data Binning

* `pd.cut()` → Converts continuous data into categorical bins

### Data Type Handling

* `df.dtypes` → Displays data types
* `astype()` → Converts data types

### Data Formatting

* `str.upper()` → Standardizes text
* `round()` → Rounds numerical values

### Data Analysis

* `value_counts()` → Counts category frequency
* `unique()` → Displays unique values

### Data Sorting

* `sort_values()` → Sorts dataset based on a column

---

## 📊 Output Summary

* Continuous data was converted into meaningful categories
* Multiple attributes were discretized for easier interpretation
* Data types were standardized
* Text data was made consistent
* Sorting improved readability and comparison
* Frequency analysis provided insight into data distribution

---

## ✅ Conclusion

The experiment demonstrates how continuous data can be effectively transformed into categorical information using data binning. Along with formatting techniques such as type conversion, standardization, and sorting, the dataset becomes more structured and easier to interpret. More importantly, discretization helps reveal underlying patterns that are not immediately visible in raw numerical data, making it a critical step in practical data analysis.

---

## 👨‍🎓 Student Details

* **Name:** Rachit Jajoo
* **PRN:** 25070123088
* **Branch:** Electronics and Telecommunication (ENTC)
* **Batch:** B1
* **Institute:** Symbiosis Institute of Technology, Pune
