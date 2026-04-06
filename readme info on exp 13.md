# Experiment 13: Data Wrangling

## 🎯 Aim

To perform preprocessing of datasets and handle missing and inconsistent values using data wrangling techniques in Python.

---

## 📚 Theory

Data wrangling is a crucial preprocessing step in data analysis where raw data is cleaned and transformed into a usable format. Real-world datasets are rarely perfect — they often contain missing values, inconsistent formats, and incorrect data types.

Effective data wrangling ensures:

* Improved data quality
* Better accuracy in analysis
* Reduced chances of misleading results

Key operations include detecting missing values, handling them appropriately, converting data types, and maintaining consistency across the dataset. The **Pandas** library provides efficient tools to perform these tasks in a structured manner.

---

## ⚙️ Commands Used & Explanation

### 🔹 Dataset 1: Missing Value Analysis

This dataset was intentionally created with missing values to understand detection and handling techniques.

#### 🔍 Detection of Missing Values

* `df1.isna()` → Identifies missing values (True = missing)
* `df1.isnull()` → Same functionality as `isna()`

#### 🔄 Detection of Valid Values

* `df1.notna()` → Identifies non-missing values
* `df1.notnull()` → Same as `notna()`

#### 🔢 Quantifying Missing Data

* `df1.isna().sum()` → Column-wise count of missing values
* `df1.isna().sum(axis=1)` → Row-wise count

👉 **Insight:** Column **C2** has the highest number of missing values, making it the most affected feature in the dataset 

#### 🗑️ Removing Missing Values

* `df1.dropna()` → Removes rows containing missing values
* `df1.dropna(axis=1)` → Removes columns containing missing values

👉 **Observation:** Dropping rows results in significant data loss, whereas dropping columns removes entire features like C1 and C2.

#### 🔧 Filling Missing Values (Imputation)

* `df1.fillna(0)` → Replaces missing values with a constant
* `df1.fillna(df1.mean())` → Uses column mean
* `df1.fillna(df1.mean(axis=1))` → Uses row-wise mean

👉 **Insight:** Mean imputation preserves dataset size and is more suitable than deletion when data loss is high.

---

### 🔹 Dataset 2: Data Cleaning & Transformation

This dataset contains inconsistent entries such as `"-"` and mixed data types.

#### 🔁 Handling Invalid Entries

* `df.replace("-", np.nan)` → Converts placeholder values into `NaN`

👉 This step standardizes missing value representation across the dataset 

#### 🔢 Data Type Conversion

* `pd.to_numeric(df["Age"], errors="coerce")`
* `pd.to_numeric(df["Marks"], errors="coerce")`

👉 Invalid entries are automatically converted into `NaN`, enabling further processing

#### 🔍 Missing Value Analysis

* `df.isna().sum()` → Displays missing values per column

👉 **Observation:** Missing values are present in **Age** and **Marks** 

#### 🧮 Imputation Techniques

* `df["Age"].fillna(df["Age"].mean())` → Mean imputation
* `df["Marks"].fillna(df["Marks"].median())` → Median imputation

👉 **Insight:** Median is preferred for marks to reduce the effect of potential outliers.

#### 🔤 Data Standardization

* `df["Department"].str.upper()` → Converts all values to uppercase

👉 Ensures uniformity in categorical data

#### 📅 Date Conversion

* `pd.to_datetime(df["Admission_Date"], errors="coerce")` → Converts to datetime format

👉 Enables proper time-based analysis and sorting

---

## 📊 Command Summary Table

| Command                 | Purpose                     |
| ----------------------- | --------------------------- |
| `isna()` / `isnull()`   | Detect missing values       |
| `notna()` / `notnull()` | Detect non-missing values   |
| `sum()`                 | Count missing values        |
| `dropna()`              | Remove missing data         |
| `fillna()`              | Replace missing values      |
| `replace()`             | Standardize invalid entries |
| `to_numeric()`          | Convert to numeric datatype |
| `str.upper()`           | Standardize text            |
| `to_datetime()`         | Convert to datetime format  |

---

## 📊 Output Summary

* Missing values were identified using boolean functions
* Column-wise analysis highlighted **C2** as the most incomplete feature
* Invalid placeholders (`"-"`) were converted to `NaN`
* Data types were corrected for numerical processing
* Missing values were handled using mean and median imputation
* Text data was standardized for consistency
* Date column was successfully converted into datetime format

---

## ✅ Conclusion

The experiment demonstrates how raw datasets can be systematically cleaned and transformed using Pandas. Instead of directly removing incomplete data, appropriate imputation techniques were applied to preserve dataset integrity. The final dataset is clean, consistent, and ready for further analysis, highlighting the importance of data preprocessing in real-world applications.

---

## 👨‍🎓 Student Details

* **Name:** Rachit Jajoo
* **PRN:** 25070123088
* **Branch:** Electronics and Telecommunication (ENTC)
* **Batch:** B1
* **Institute:** Symbiosis Institute of Technology, Pune
