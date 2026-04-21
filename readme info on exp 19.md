# 📊 Experiment 19: Real World and Interactive Visualizations

---

## 🎯 Aim

To study and implement real world and interactive visualization techniques using Python libraries such as Plotly, Matplotlib, Pandas, NumPy, SciPy, and Matplotlib-Venn for representing hierarchical data, clustering, set relationships, flow systems, multivariable analysis, and performance comparison.

---

## 📚 Theory

Data visualization is one of the most powerful tools in modern analytics. While basic charts such as bar graphs and line plots are useful for simple comparisons, many real-world problems require more advanced visualization techniques that can represent hierarchy, relationships, clustering, movement, and multi-dimensional data.

Interactive charts further improve analysis by allowing users to:

- Hover over data points  
- Zoom in and out  
- Rotate 3D graphs  
- Filter information dynamically  
- Explore patterns in detail  

This experiment focuses on advanced and interactive charts commonly used in business dashboards, machine learning, finance, education systems, and management analytics.

The libraries used are:

- **Plotly Express** → Easy creation of interactive charts  
- **Plotly Graph Objects** → Advanced custom visualizations  
- **Matplotlib** → Static plotting library  
- **Pandas** → Dataset creation and tabular data handling  
- **NumPy** → Numerical arrays and sample data generation  
- **SciPy** → Hierarchical clustering algorithms  
- **Matplotlib-Venn** → Venn diagram creation  

---

## 🔹 1. Treemap

A Treemap is used to visualize hierarchical data using rectangles. Each rectangle represents a category, and its size is proportional to a numerical value.

The example used department budget allocation:

- HR  
- IT  
- Sales  
- Marketing  

The chart was created using `px.treemap()`.

Parameters used:

- `path=` → Defines hierarchy labels  
- `values=` → Determines rectangle area  

Larger rectangles indicate larger budgets.

### Real World Applications

- Company budget allocation  
- Product sales by category  
- Portfolio investment breakdown  
- Storage space analysis  

Treemaps are preferred when many categories must be compared compactly.

---

## 🔹 2. Dendrogram

A Dendrogram is a tree-like chart used in hierarchical clustering.

It shows how similar data points merge into clusters step-by-step. The vertical axis represents distance or dissimilarity between groups.

The following functions were used:

- `linkage(data, method='ward')` → Performs clustering  
- `dendrogram()` → Displays cluster tree  

The Ward method minimizes variance within clusters.

### Real World Applications

- Customer segmentation  
- Gene analysis  
- Pattern recognition  
- Recommendation systems  
- Image classification  

Dendrograms are important in unsupervised machine learning.

---

## 🔹 3. Venn Diagram

A Venn Diagram is used to represent relationships between sets using overlapping circles.

The example used:

- Set A = {1,2,3,4}  
- Set B = {3,4,5,6}

This displays:

- Unique values in Set A  
- Common values in both sets  
- Unique values in Set B  

The chart was created using `venn2()`.

### Real World Applications

- Database query operations  
- Mathematics and probability  
- Common skills between teams  
- Customer overlap between markets  

Venn diagrams make set logic easy to understand visually.

---

## 🔹 4. Sankey Diagram

A Sankey Diagram is used to represent flow from one stage to another.

The example tracked student movement through stages:

- Admission  
- First Year  
- Second Year  
- Placed  

Flow values:

- 100 students entered Admission  
- 80 progressed further  
- 60 reached placement stage  

The chart was created using `go.Sankey()`.

In Sankey diagrams, the thickness of links represents quantity.

### Real World Applications

- Student retention analysis  
- Supply chain movement  
- Energy transfer systems  
- Budget expenditure flow  
- Website user journey analysis  

Sankey diagrams are excellent for showing loss, gain, or movement through processes.

---

## 🔹 5. 3D Scatter Plot

A 3D Scatter Plot is used when three numerical variables need to be visualized simultaneously.

The dataset contained:

- Study_Hours  
- Marks  
- Attendance  

Axes used:

- X-axis → Study Hours  
- Y-axis → Marks  
- Z-axis → Attendance  

The chart was created using `px.scatter_3d()`.

Since Plotly is interactive, users can rotate and inspect the graph from different angles.

### Real World Applications

- Student performance analytics  
- Scientific experiments  
- Production quality analysis  
- Financial risk modeling  

This chart reveals patterns that may not be visible in 2D graphs.

---

## 🔹 6. Radar Chart

A Radar Chart (Spider Chart) is used to compare multiple performance indicators on radial axes.

The example evaluated skills:

- Python  
- ML  
- DBMS  
- DSA  
- Communication  

The chart was created using `go.Scatterpolar()`.

The parameter:

- `fill='toself'`

fills the polygon area enclosed by skill scores.

### Real World Applications

- Student skill assessment  
- Employee appraisal systems  
- Product feature comparison  
- Sports player analysis  

Radar charts quickly highlight strengths and weaknesses.

---

## 🔹 7. Importance of Interactive Visualization using Plotly

Unlike static graphs, Plotly charts offer:

- Hover tooltips  
- Zoom controls  
- Pan and rotate features  
- Dynamic legends  
- Better presentation quality  

This makes Plotly highly valuable in dashboards and business reporting.

---

## 📊 Output Summary

The following visualizations were successfully generated:

- Treemap  
- Dendrogram  
- Venn Diagram  
- Sankey Diagram  
- 3D Scatter Plot  
- Radar Chart  

---

## 📈 Comparison of Visualization Types

| Visualization Type | Main Purpose |
|-------------------|-------------|
| Treemap | Hierarchical comparison |
| Dendrogram | Cluster analysis |
| Venn Diagram | Set relationships |
| Sankey Diagram | Flow analysis |
| 3D Scatter Plot | Three-variable relationship |
| Radar Chart | Multi-metric comparison |

---

## 🚀 Learning Outcomes

- Learned advanced real-world visualization techniques  
- Understood hierarchical and clustering charts  
- Learned flow-based and interactive diagrams  
- Explored multi-dimensional data representation  
- Understood how Plotly improves dashboard quality  
- Learned practical business uses of specialized charts  

---

## ✅ Conclusion

The experiment successfully demonstrated real world and interactive visualization techniques using Python. Treemap, dendrogram, Venn diagram, Sankey diagram, 3D scatter plot, and radar chart were implemented using Plotly, Matplotlib, SciPy, and Pandas. These charts are highly valuable for analytics, business intelligence, machine learning, education systems, and decision-making dashboards where complex data must be communicated clearly and effectively.

---

## 👨‍🎓 Student Details

- **Name:** Rachit Jajoo  
- **PRN:** 25070123088  
- **Branch:** Electronics and Telecommunication (ENTC)  
- **Batch:** B1  
- **Institute:** Symbiosis Institute of Technology, Pune
