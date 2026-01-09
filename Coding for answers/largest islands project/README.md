# 🏝️ World’s Largest Islands  
### Exploratory Geographic Data Analysis  
*(Part of My Data Analytics & Data Science Portfolio)*

## 🔎 Project Overview

This project presents an **exploratory data analysis of the world’s largest islands** using structured geographic data.  
The analysis focuses on island size, regional distribution, tropical presence, and political composition.

The notebook is designed to demonstrate **core data analysis workflows** including data ingestion, sorting, grouping, visualization, and string-based filtering using Python.

---

## 🎯 Analytical Objectives

The analysis addresses the following questions:

1. What are the **10 largest islands in the world**?
2. What is the **largest island in each geographic region**?
3. How does island **area vary with rank**?
4. Which islands are **shared by multiple countries**?

---

## 📂 Dataset Used

- **`largest-islands.csv`**

### Dataset Fields
- `name` – Island name  
- `area` – Area in square kilometers (km²)  
- `rank` – Global rank by size  
- `region` – Geographic region  
- `countries` – Country or countries governing the island  

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- Matplotlib
- Jupyter Notebook / Google Colab

---

## 🔬 Analysis Performed

### 1. Data Loading & Inspection
- Loaded the dataset using Pandas
- Inspected structure and sample rows using `head()`

### 2. Largest Islands by Area
- Sorted islands by `area` in descending order
- Extracted the **top 10 largest islands globally**

### 3. Largest Island by Region
- Grouped data by `region`
- Identified the largest island within each region using sorted grouping

### 4. Rank vs Area Visualization
- Created a **line graph** with:
  - X-axis: Island rank (largest to smallest)
  - Y-axis: Island area (km²)
- Used Matplotlib for visualization

### 5. Multi-Country Islands
- Identified islands governed by **multiple countries**
- Used string pattern matching (`str.contains(',')`) on the `countries` column

---

## 📈 Key Observations

- Island size drops sharply after the highest-ranked islands
- Certain regions are dominated by a single very large island
- Several large islands span **multiple countries**, reflecting geopolitical complexity
- Ranking and area have a strong, non-linear relationship

---

## 📁 Repository Structure

```text
├── World's largest islands.ipynb
├── largest-islands.csv
└── README.md
````

---

## 🚀 How to Run

1. Clone the repository
2. Open the notebook in **Jupyter Notebook** or **Google Colab**
3. Ensure `largest-islands.csv` is in the same directory
4. Run cells sequentially

---

## 🧠 Portfolio Relevance

This project demonstrates:

* Clean exploratory data analysis
* Sorting, grouping, and aggregation logic
* Basic but effective data visualization
* Ability to translate geographic questions into data queries

It complements other portfolio projects focused on:

* Global datasets
* Scientific and geographic analysis
* Structured exploratory workflows

---

## 👤 Author

**Bhavik Buchke**
| Data Scientist

---

⭐ *This repository is part of a continuously evolving GitHub data science portfolio.*
