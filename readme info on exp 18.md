# 📊 Experiment 18: Exploring Statistical and Specialized Data Visualization Techniques

---

## 🎯 Aim

To study and implement statistical and specialized data visualization techniques using Python libraries such as Matplotlib, Seaborn, Pandas, and NumPy.

---

## 📚 Theory

Data visualization is an important part of data analysis. It helps convert raw numerical information into meaningful graphical representations so that patterns, trends, correlations, and outliers can be easily understood.

Apart from basic charts such as line graphs and bar charts, advanced visualization techniques like area plots, pie charts, donut charts, boxplots, heatmaps, and bubble plots are widely used in analytics and business intelligence.

The libraries used in this experiment are:

- **Matplotlib** → Core plotting library for Python  
- **Seaborn** → Statistical visualization library built on Matplotlib  
- **Pandas** → Used for dataset creation and manipulation  
- **NumPy** → Used for random values and numerical operations  

---

### 🔹 1. Dataset Creation using Pandas and NumPy

A sample dataset was created using `pd.DataFrame()` with fixed random values using `np.random.seed(0)` for reproducibility.

The dataset contained:

- **Category** → A, B, C, D, E  
- **Values** → Numeric values used for charts  
- **Sales** → Random sales values  
- **Profit** → Random profit values  

The command `np.random.randint()` was used to generate random integers.

Using a fixed random seed ensures the same random values appear each time the program runs.

---

### 🔹 2. Area Plot

An Area Plot is used to represent quantitative data with the area below the line filled with color.

The command `plt.fill_between(x, y)` was used to fill the region between x-axis and data values.

Parameters used:

- `color='green'` → Fill color  
- `alpha=0.25` → Transparency level  

This chart was used to plot **Category vs Values**.

Area plots are useful for showing magnitude over categories or time.

---

### 🔹 3. Multiple Area Plot (Sales and Profit)

Two filled area graphs were plotted together for comparison.

The command `plt.fill_between()` was used separately for:

- Sales  
- Profit  

Different colors were used:

- Skyblue → Sales  
- Orange → Profit  

The command `plt.legend()` was used to identify each region.

Seaborn style was applied using:

- `sns.set_style("whitegrid")`

This chart helps compare two continuous datasets visually.

---

### 🔹 4. Pie Chart

A Pie Chart represents parts of a whole using sectors of a circle.

The command `plt.pie(values, labels=labels, autopct=)` was used.

Parameters:

- `labels=` → Category names  
- `autopct='%1.2f%%'` → Displays percentage with two decimal places  

This chart showed the contribution of each category to total values.

Pie charts are useful for percentage composition analysis.

---

### 🔹 5. Donut Chart

A Donut Chart is a modified pie chart with a hollow center.

It was created using a pie chart and adding a white center circle using:

- `plt.Circle((0,0), 0.70, fc='white')`

The command `fig.gca().add_artist()` placed the center circle.

This chart improves visual appearance and creates space in the center for labels if needed.

---

### 🔹 6. Boxplot (Outlier Detection)

A Boxplot is used to summarize distribution and detect outliers.

The command `sns.boxplot(x=data)` was used.

It displays:

- Minimum value  
- First Quartile (Q1)  
- Median  
- Third Quartile (Q3)  
- Maximum value  
- Outliers (if present)

This chart was created using the Values column.

Boxplots are useful for statistical summaries and anomaly detection.

---

### 🔹 7. Heatmap (Correlation Matrix)

A Heatmap visually represents correlation values using colors.

The command:

- `df[['Sales','Profit']].corr()`

was used to calculate correlation matrix.

Then:

- `sns.heatmap(corr, annot=True, cmap='coolwarm')`

was used to display it.

Parameters:

- `annot=True` → Shows numeric correlation values  
- `cmap='coolwarm'` → Color theme

This chart helps understand relationships between variables.

---

### 🔹 8. Extended Heatmap using Multiple Columns

Another heatmap was created using:

- Values  
- Sales  
- Profit  

The command `.corr()` automatically selected relationships among numeric columns.

The chart displayed positive and negative correlations among all selected variables.

Heatmaps are widely used in machine learning and feature selection.

---

### 🔹 9. Bubble Plot using Matplotlib

A Bubble Plot is an extended scatter plot where bubble size represents a third variable.

The command:

- `plt.scatter(x, y, s=size)`

was used.

Where:

- X-axis = Sales  
- Y-axis = Profit  
- Bubble Size = Values × 10

The parameter `s=` controls marker size.

This allows three variables to be represented in one graph.

---

### 🔹 10. Bubble Plot using Seaborn

A more advanced bubble plot was created using:

- `sns.scatterplot()`

Parameters used:

- `x='Sales'`
- `y='Profit'`
- `size='Values'` → Bubble size  
- `hue='Values'` → Bubble color  
- `sizes=(50,300)` → Minimum and maximum size range  
- `palette='viridis'` → Color palette

This chart provides clearer and more attractive visual encoding.

---

## 📊 Output Summary

The following visualizations were successfully generated:

- Area Plot  
- Multiple Area Plot  
- Pie Chart  
- Donut Chart  
- Boxplot  
- Heatmap  
- Multi-variable Heatmap  
- Bubble Plot using Matplotlib  
- Bubble Plot using Seaborn  

---

## 📈 Importance of Specialized Charts

| Chart Type | Main Use |
|-----------|----------|
| Area Plot | Trend with magnitude |
| Pie Chart | Percentage contribution |
| Donut Chart | Improved pie chart visualization |
| Boxplot | Outlier detection |
| Heatmap | Correlation analysis |
| Bubble Plot | Three-variable comparison |

---

## ✅ Conclusion

The experiment successfully demonstrated advanced statistical and specialized data visualization techniques using Python. Area plots, pie charts, donut charts, boxplots, heatmaps, and bubble plots were implemented using Matplotlib and Seaborn. These charts are highly useful in data analytics for understanding composition, correlation, distribution, and multivariable relationships.

---

## 👨‍🎓 Student Details

- **Name:** Rachit Jajoo  
- **PRN:** 25070123088  
- **Branch:** Electronics and Telecommunication (ENTC)  
- **Batch:** B1  
- **Institute:** Symbiosis Institute of Technology, Pune

---
```
