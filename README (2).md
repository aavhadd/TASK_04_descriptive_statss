# Task_03_Descriptive_Stats

This repository contains my work for Syracuse University OPT Research Task 3. The objective was to analyze datasets related to advertising spend and social media activity on Facebook and Twitter during the 2024 U.S. Presidential Election, using:

- Pure Python (no third-party libraries)  
- Pandas  
- Polars  

A bonus section includes exploratory visualizations designed to support presentation to senior stakeholders.

---

## 📂 Project Structure

```
Task_03_Descriptive_Stats/
│
├── pure_python_stats.py
├── pandas_stats.py
├── polars_stats.py
├── visualization.ipynb
├── .gitignore
└── README.md
```

---

## How to Run the Scripts

All three main scripts are **parameterized**. You can run them on any of the three datasets by specifying:

1. The CSV filename  
2. The grouping columns for that dataset

Below you'll find **step-by-step** instructions **for each dataset**, **for each approach**.

---


## 📂 Public Data Sources

- World University Rankings
  - [https://www.kaggle.com/datasets/mylesoneill/world-university-rankings](https://www.kaggle.com/datasets/mylesoneill/world-university-rankings)
  - Example grouping column: "country"

- Global Superstore Orders
  - [https://www.kaggle.com/datasets/vivek468/superstore-dataset-final](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
  - Example grouping columns: "Country", "Category"

- US Census County Population Estimates
  - [https://www2.census.gov/programs-surveys/popest/datasets/2020-2023/counties/totals/co-est2023-alldata.csv](https://www2.census.gov/programs-surveys/popest/datasets/2020-2023/counties/totals/co-est2023-alldata.csv)
  - Example grouping column: "STATE"
  - 


## ✅ How to Run

### 📌 World University Rankings
python pure_python_stats.py cwurData.csv "country"
python pandas_stats.py cwurData.csv "country"
python polars_stats.py cwurData.csv "country"

### 📌 Global Superstore Orders
python "pure_python_stats.py" "Sample - Superstore.csv" "Country" "Category"
python "pandas_stats.py" "Sample - Superstore.csv" "Country" "Category"
python "polars_stats.py" "Sample - Superstore.csv" "Country" "Category"

### 📌 US Census County Population Estimates
python pure_python_stats.py co-est2023-alldata.csv "STATE"
python pandas_stats.py co-est2023-alldata.csv "STATE"
python polars_stats.py co-est2023-alldata.csv "STATE"



## ✅ Short Summary of Findings

### 📌 World University Rankings
- Countries show wide variance in teaching and research scores.
- Some universities have exceptionally high citations.
- Distribution is right-skewed with high outliers.

### 📌 Global Superstore Orders
- Sales and profit are highly skewed.
- Certain countries and categories dominate total sales.
- Discounts are unevenly applied across categories.

### 📌 US Census County Population Estimates
- Most counties have small populations.
- Populations are heavily concentrated in a few states.
- Data distribution requires log scale visualization for clarity.


## 📊 Bonus: Visualization Notebook


designed to create clear, presentation-ready charts for **all three datasets**:

✅ World University Rankings  
✅ Global Superstore Orders  
✅ US Census County Population Estimates

---

### ⚡️ How to Use

1️⃣ Open Jupyter Notebook in your project folder  
2️⃣ Launch `Visualization.ipynb`  
3️⃣ Choose which dataset to load (edit the path in the notebook if needed)  
4️⃣ Run the cells top-to-bottom

✅ All plots will render **inline** in the notebook.  
✅ You can rerun cells or adjust parameters as you explore.

---

### 📌 Included Visualizations

#### ✅ 1️⃣ Histograms
- Distribution of numeric columns
- Optional KDE overlays
- Highlights skewness and outliers

#### ✅ 2️⃣ Boxplots
- Compare numeric metrics by category
- For example:
  - University scores by country
  - Sales or Profit by Category or Country
  - Population estimates by State

#### ✅ 3️⃣ Bar Charts
- Top N categories by count or sum
- For example:
  - Top 10 countries with most universities
  - Top 10 customer countries in Superstore
  - Top states by number of counties

#### ✅ 4️⃣ Correlation Heatmaps
- Numeric feature correlations
- Helps spot relationships among variables

#### ✅ 5️⃣ Plotly Interactive Charts
- Interactive histograms and boxplots
- Click, zoom, and hover tooltips for rich storytelling

---

### ✅ Example Usage for Each Dataset

#### 📌 World University Rankings
- Histogram of research, citations, and teaching scores
- Boxplot of score by country
- Top 10 countries by university count
- Correlation heatmap of scores

#### 📌 Global Superstore Orders
- Histograms of Sales and Profit
- Boxplots of Profit by Category and Country
- Bar charts for top-selling countries or categories
- Interactive sales and profit distributions

#### 📌 US Census County Population Estimates
- Histogram of county-level population estimates
- Boxplot of population by State
- Bar chart of total state population
- Log-scale plots to reveal spread

---

### ✅ 📌 Purpose

This notebook is designed to:

✔️ Enable exploratory data analysis (EDA)  
✔️ Reveal trends, patterns, and outliers  
✔️ Create **presentation-ready** charts for stakeholders  
✔️ Support **data storytelling** for researchers and executives

---

### ✅ Notes

- You can **customize** grouping columns, color palettes, and bin sizes directly in the notebook cells.  
- Plots can be saved as PNG or shared interactively.  
- Designed for **in-depth research presentations** or quick one-off data checks.

---

