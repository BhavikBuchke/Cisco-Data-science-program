# Banknote Dimensions: Global Accessibility & Practicality Analysis

> **Created as part of the Cisco Data Science Program.**

## 📊 Executive Summary

In the world of currency design, banknote dimensions are far more than just a matter of aesthetics. They represent a critical intersection between **accessibility** (assisting the visually impaired) and **operational efficiency** (compatibility with ATMs and vending machines).

This project analyzes a dataset of 42 global currencies to identify patterns in physical dimensions. By leveraging Python's data analysis stack, we identify which nations prioritize uniform dimensions for machine processing and which utilize varied sizes to enhance tactile distinguishability for their citizens.

---

## 🎯 The Business Problem

Currency designers face a constant trade-off:

1. **Uniformity:** Enhances durability and ensures seamless processing by high-speed sorting machines and ATMs.
2. **Variability:** Vital for the visually impaired to differentiate between denominations by touch and size.

**The Goal:** To quantify these differences across 42 currencies and categorize global trends in banknote physical architecture using statistical visualization.

---

## 💡 Key Insights & Results

Through the analysis of the `banknote-dimensions.csv` dataset, the following findings were observed:

| Dimension Pattern | Currency Examples | Impact |
| --- | --- | --- |
| **Uniform Sizing** | Argentine Peso, Canadian Dollar | Optimized for durability and machine sorting; lower accessibility for visually impaired. |
| **Length Variation Only** | Australian Dollar, Chinese Yuan | Balanced approach; uses length increments to signify value increase. |
| **Full Size Scaling** | Euro, Bangladeshi Taka | Maximum accessibility; both height and width scale with value for easy tactile recognition. |

* **The Largest Overall:** The **Czech Koruna** and **Euro (500 note)** feature some of the largest dimensions in the dataset (up to 170mm in length).
* **The Size Gaps:** Currencies like the **Bangladeshi Taka** exhibit a massive 55mm difference between the smallest and largest notes, significantly aiding manual sorting.

---

## 🛠 Technical Workflow

### 1. Data Processing & Cleaning

Using `pandas`, the raw dataset was inspected for consistency. We performed grouping operations to isolate the `max` and `min` dimensions for every currency in the dataset to calculate the "Size Spread" for each nation.

### 2. Feature Engineering

Created a `diff` feature to represent the absolute difference in millimeters between a currency's highest and lowest denomination. This serves as a proxy for how "accessible" a currency system is designed to be.

### 3. Exploratory Data Visualization

Developed paired scatter plots and categorical bar charts using `matplotlib` to analyze:

* **Min vs. Max Length/Width:** To visualize the variance in physical size.
* **Consistency Ratios:** To determine the percentage of global currencies following specific design philosophies.

---

## 📈 Visualizations

### 1. Length & Width Variance

These scatter plots compare the smallest and largest notes for each currency. Currencies sitting on the diagonal line have uniform dimensions, while those further away offer high tactile variance for accessibility.

<img width="500" height="300" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/64394d7a-1541-4900-a77f-840db71e9e2f" />
<img width="500" height="300" alt="Code_Generated_Image(1)" src="https://github.com/user-attachments/assets/d8dee5ea-e1d0-4a63-9d25-a511072579c5" />


### 2. Global Consistency Trends

The bar chart below illustrates how common each design strategy is across the 42 sampled currencies. A significant portion of currencies maintain a consistent width while varying length.

<img width="500" height="300" alt="Code_Generated_Image(2)" src="https://github.com/user-attachments/assets/6c650a7c-67c1-49ac-974d-3e3aae98d68d" />

---

## 🚀 How to Run

To explore the analysis and generate the visualizations locally:

1. **Clone the repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data visualization/Banknote Dimensions Project"

```


2. **Install dependencies:**
```bash
pip install pandas matplotlib

```


3. **Launch the Notebook:**
```bash
jupyter notebook "banknote dimensions.ipynb"

```



---

## 📂 Project Structure

* `banknote dimensions.ipynb`: The main analytical engine containing Python code and visualizations.
* `banknote-dimensions.csv`: The raw dataset containing dimensions for 42 global currencies.
* `length_analysis.png`: Scatter plot of length variance.
* `width_analysis.png`: Scatter plot of width variance.
* `dimension_consistency.png`: Bar chart of design philosophy distribution.

---

*Developed with a focus on data storytelling and visual clarity.*
