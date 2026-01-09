# 🎨 Art as Data  
### Structured Analysis of Piet Mondrian Paintings  
*(Part of My Data Analytics & Data Science Portfolio)*

---

## ✅ What the Notebook Actually Does

This notebook performs a **structured exploratory analysis of abstract art data**, using datasets derived from **Piet Mondrian’s paintings**.

Specifically, the notebook:

- Loads **three CSV datasets** containing painting metadata and geometric features
- Examines how **rectangular elements** are distributed within paintings
- Uses **painting IDs** to group and compare features
- Computes summary statistics (counts, averages) of visual components
- Compares a **single painting (FP26)** against the broader dataset
- Demonstrates how **visual art can be represented and analyzed as tabular data**

The notebook does **not**:
- Train machine learning models
- Perform image processing
- Conduct statistical hypothesis testing

This is a **pure exploratory data analysis (EDA)** notebook grounded in structured feature data.

---

## 🔎 Project Overview

This project explores how **abstract art can be treated as data** by analyzing numerical and categorical features extracted from paintings.  
Using datasets related to Piet Mondrian’s work, the notebook applies standard data analysis techniques to understand how individual paintings are composed and how they compare to one another.

The goal is to demonstrate that **data science workflows apply meaningfully outside traditional business domains**.

---

## 📂 Datasets Used

The notebook works with the following datasets:

- **`mondrian-painting-features.csv`**  
  Contains geometric features (e.g., rectangles) associated with Mondrian paintings.  
  Each painting appears in multiple rows—one per visual element.

- **`mondrian-painting-info.csv`**  
  Contains metadata about each painting, such as identifiers and descriptive attributes.

- **`fp26-features.csv`**  
  Feature-level data for a specific painting (FP26), used for focused comparison.

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- Jupyter Notebook / Google Colab

---

## 🔬 Analysis Performed

### 1. Data Loading & Inspection
- Loaded all datasets using Pandas
- Inspected structure and confirmed that paintings are represented by **multiple rows per ID**

### 2. Painting-Level Feature Exploration
- Used `query()` to extract all features associated with a single painting
- Examined how many geometric elements make up one artwork

### 3. Grouped Analysis by Painting ID
- Grouped feature data by `painting_id`
- Computed counts and summary statistics per painting
- Compared individual paintings against dataset-wide patterns

### 4. Focused Comparison: FP26
- Loaded a dedicated dataset for painting FP26
- Compared FP26’s feature composition to the broader Mondrian dataset

All operations are implemented using Pandas transformations such as:
- `query`
- `groupby`
- `count`
- `mean`
- DataFrame filtering and inspection

---

## 📈 Key Observations

- Individual paintings consist of **multiple geometric elements**, each represented as a row
- Paintings vary significantly in the number and composition of rectangular features
- A single artwork (FP26) can be meaningfully compared to an entire collection using summary statistics
- Abstract art can be effectively analyzed using structured, tabular data

These observations are derived directly from computed outputs in the notebook.

---

## 📁 Repository Structure

```text
├── art as data.ipynb
├── mondrian-painting-features.csv
├── mondrian-painting-info.csv
├── fp26-features.csv
└── README.md
````

---

## 🚀 How to Run

1. Clone the repository
2. Open the notebook in **Jupyter Notebook** or **Google Colab**
3. Upload or place all CSV files in the working directory
4. Run cells sequentially

---

## 🧠 Portfolio Relevance

This project demonstrates:

* Strong fundamentals in exploratory data analysis
* Ability to reason about **non-traditional datasets**
* Experience working with one-to-many relational data
* Clean, interpretable Pandas workflows

It complements other portfolio projects focused on:

* Global and geographic data
* Scientific and research-oriented analysis
* Consumer and design-based datasets

---

## 👤 Author

**Bhavik Buchke**
| Data Scientist

---

⭐ *This repository is part of a continuously evolving GitHub data science portfolio.*
