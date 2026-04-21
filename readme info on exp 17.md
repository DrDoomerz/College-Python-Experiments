# 📊 Experiment 17: Basic Charts and Visual Encoding in Python

---

## 🎯 Aim

To study and implement various basic charts and visual encoding techniques using Python libraries such as Matplotlib, Seaborn, Pandas, and NumPy for effective graphical representation of data.

---

## 📚 Theory

Data Visualization is the graphical representation of data using charts, graphs, and plots. It helps convert raw numerical information into meaningful visuals so that trends, comparisons, relationships, and distributions can be understood easily.

Python provides several powerful libraries for visualization:

- **Matplotlib** → Fundamental plotting library used for creating static charts.
- **Seaborn** → Advanced statistical visualization library built on Matplotlib.
- **Pandas** → Used for creating and handling structured datasets.
- **NumPy** → Used for numerical calculations such as mean and averages.

This experiment demonstrates multiple chart types and visual encoding methods using these libraries.

---

### 🔹 1. Dataset Creation using Pandas

A structured dataset was created using Python dictionaries and converted into a DataFrame using `pd.DataFrame()`.

The dataset contained the following fields:

- Days  
- Study_Hours  
- Marks  
- Attendance  
- Sleep_Hours  
- Assignments_Completed  

This student dataset was used for line charts, bar charts, histograms, and scatter plots.

Another business dataset was also created containing:

- Days  
- Region  
- Sales  
- Profit  
- Customers  
- Category  

This dataset was used for Seaborn visualizations.

---

### 🔹 2. Line Chart

A line chart is used to show trends or changes across time or categories.

The command `plt.plot(x, y)` was used to connect data points with straight lines. Markers such as `marker='*'` were used to highlight each point.

The line chart plotted **Study Hours vs Days**, helping visualize how study time changed during the week.

Additional functions used:

- `plt.title()` → Adds chart title  
- `plt.xlabel()` → Labels x-axis  
- `plt.ylabel()` → Labels y-axis  
- `plt.show()` → Displays graph

---

### 🔹 3. Multi-Line Chart

Multiple lines can be drawn on the same graph by using `plt.plot()` more than once.

Study Hours and Marks were plotted together using different colors and markers. The command `plt.legend()` was used to identify each line.

This chart helps compare two variables simultaneously.

The command `plt.figure(figsize=(7,4))` was used to set chart size.

---

### 🔹 4. Bar Chart

A bar chart compares values among categories using rectangular bars.

The command `plt.bar(x, y)` was used to plot **Marks vs Days**.

Bar charts are useful when comparing discrete categories such as marks across weekdays.

The parameter `color='green'` was used to style bars.

---

### 🔹 5. Bar Chart with Value Labels

An advanced bar chart was created where numerical values were displayed above each bar.

This was achieved using:

- `bar.get_height()` → Retrieves height of each bar  
- `plt.text()` → Writes text above bars

The command `plt.grid(axis='y')` added horizontal grid lines for better readability.

This type of chart gives both visual and exact numerical comparison.

---

### 🔹 6. Histogram

A histogram is used to show frequency distribution of continuous numerical data.

The command `plt.hist(data, bins=5)` grouped marks into intervals.

Other parameters used:

- `bins=5` → Number of groups  
- `edgecolor='black'` → Black borders around bars  
- `alpha=0.7` → Transparency level

This chart helps understand spread and concentration of marks.

---

### 🔹 7. Histogram with Mean Line

A more informative histogram was created by adding a vertical mean reference line.

The mean was calculated using:

- `np.mean(data)`

The command:

- `plt.axvline(mean_value)`

was used to draw a vertical dashed red line showing average marks.

Additional styling:

- `linestyle='--'`
- `linewidth=2`

This chart helps compare data distribution with average value.

---

### 🔹 8. Scatter Plot

A scatter plot displays relationship between two numerical variables.

The command `plt.scatter(x, y)` was used to plot:

- Study Hours vs Marks

Each point represents one observation.

When points move upward from left to right, it indicates positive correlation.

This graph is useful for studying relationships between variables.

---

### 🔹 9. Conditional Scatter Plot (Visual Encoding)

Visual encoding means using visual properties such as color, shape, or size to represent extra information.

A scatter plot was created where points were colored according to result:

- Red → Fail  
- Green → Pass  

This was done using the `c=` parameter of `plt.scatter()`.

Thus, three variables were represented in one chart:

- X-axis = Study Hours  
- Y-axis = Marks  
- Color = Result

---

### 🔹 10. Seaborn Line Plot

The command `sns.lineplot(x=, y=, data=)` was used to create a line chart of **Sales vs Days**.

Seaborn automatically creates cleaner and more professional charts than basic Matplotlib.

This chart was used to visualize sales trend.

---

### 🔹 11. Seaborn Histogram

The command `sns.histplot(data, kde=True)` was used to plot Sales distribution.

The parameter:

- `kde=True`

adds a smooth density curve over the histogram.

This helps understand the shape of data distribution.

---

### 🔹 12. Seaborn Scatter Plot

The command `sns.scatterplot(x=, y=, data=)` was used to plot:

- Sales vs Profit

This chart helps identify whether higher sales lead to higher profit.

Seaborn charts are more visually appealing and easier to interpret.

---

## 📊 Output Summary

The following visualizations were successfully generated:

- Line Chart  
- Multi-Line Comparison Chart  
- Bar Chart  
- Labelled Bar Chart  
- Histogram  
- Histogram with Mean Line  
- Scatter Plot  
- Conditional Scatter Plot  
- Seaborn Line Plot  
- Seaborn Histogram  
- Seaborn Scatter Plot  

---

## 📈 Comparison: Matplotlib vs Seaborn

| Feature | Matplotlib | Seaborn |
|--------|------------|---------|
| Customization | High | Medium |
| Simplicity | Medium | High |
| Appearance | Basic | Attractive |
| Statistical Charts | Limited | Excellent |

---

## ✅ Conclusion

The experiment successfully demonstrated various chart types and visual encoding techniques using Python. Matplotlib provided highly customizable graphs, while Seaborn produced cleaner statistical visuals. These tools are essential in data analysis for representing trends, comparisons, distributions, and relationships effectively.

---

## 👨‍🎓 Student Details

- **Name:** Rachit Jajoo  
- **PRN:** 25070123088  
- **Branch:** Electronics and Telecommunication (ENTC)  
- **Batch:** B1  
- **Institute:** Symbiosis Institute of Technology, Pune

---
```
