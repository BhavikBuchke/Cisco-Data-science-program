# World Population Distribution: 1800 – 2100 Analysis

> **Analyzing the past to understand the future of our global community.**

## 📊 Executive Summary

Understanding demographic shifts is fundamental to global economics, resource management, and policy-making. This project explores the historical and projected population distribution across four major global regions: **Africa, Asia, the Americas, and Europe**.

Using longitudinal data from 1800 to 2100 (projected), this analysis highlights the transition from a world dominated by European and Asian population shares to one where African demographics represent a significantly larger portion of the global total. The project demonstrates advanced data pivoting, custom visualization styling, and time-series storytelling.

---

## 🎯 The Business Problem

Global businesses and NGOs must anticipate where future demand, labor, and social needs will arise.

* **The Problem:** Raw population data is often difficult to interpret across long time horizons due to differing growth rates.
* **The Goal:** To visualize regional "growth trajectories" and quantify the shift in regional dominance by the end of the 21st century.

---

## 💡 Key Insights & Results

The analysis reveals several critical demographic inflection points:

| Region | 2000 Population | 2100 Projection | Analysis |
| --- | --- | --- | --- |
| **Asia** | ~3.7 Billion | **~4.7 Billion** | Remains the most populous, but growth slows significantly by 2050. |
| **Africa** | ~0.8 Billion | **~3.9 Billion** | The fastest-growing region; expected to nearly quadruple its population. |
| **Americas** | ~0.8 Billion | ~1.1 Billion | Steady, moderate growth followed by late-century stabilization. |
| **Europe** | ~0.7 Billion | ~0.6 Billion | The only region projected to see a **population decline**. |

* **Regional Dominance Shift:** By 2100, Africa and Asia will combined house nearly **80% of the world's population**.
* **The Peak:** Most regions reach a "plateau" in the late 21st century, except for Africa, which continues its upward trajectory throughout the projection period.

---

## 🛠 Technical Workflow

### 1. Data Cleaning

The raw `world-indicators.csv` contains numerous socioeconomic metrics. We specifically isolated `year`, `region`, and `population`. Data was filtered to exclude the aggregate "world" entry to focus specifically on regional comparisons.

### 2. Feature Engineering

Population counts were converted from raw integers to **Billions** (`pop_billions`) to improve readability and ensure visualizations were not cluttered with scientific notation.

### 3. Data Transformation

Used `df.pivot()` to restructure the data from a "long" format into a "wide" format. This transformation is essential for time-series plotting, allowing each region to be represented as a distinct line in a single plot.

### 4. Custom Visualization Design

The project implements a "Pro-Tip" design philosophy:

* **Minimalist Styling:** Removed unnecessary "chart junk" (top/right spines) to focus the viewer's eye on the data.
* **End-Labeling:** Instead of a traditional legend, custom helper functions label lines directly at their terminus for immediate identification.

---

## 📈 Visualizations

### 1. Longitudinal Growth (1800-2100)

This line plot tracks the rise of regional populations over three centuries. Note the sharp divergence in growth between Africa and the other regions starting in the late 20th century.

<img width="900" height="450" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/255c283e-bfa3-41e6-9e8d-bdde86467054" />

### 2. Regional Comparison: 2000 vs. 2100

These horizontal bar charts provide a "snapshot" comparison between the start of the millennium and the projected end, emphasizing the massive expansion of the African demographic footprint.

<img width="900" height="500" alt="Code_Generated_Image(1)" src="https://github.com/user-attachments/assets/43492218-bf56-4509-bccd-f5aaad14ac0c" />

---

## 🚀 How to Run

To run this analysis on your local machine:

1. **Clone the repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data visualization/Continent Populations Project"

```


2. **Install requirements:**
```bash
pip install pandas matplotlib

```


3. **Execute the Notebook:**
```bash
jupyter notebook "Continent populations.ipynb"

```



---

## 📂 Project Structure

* `Continent populations.ipynb`: Complete Python source code and analysis.
* `world-indicators.csv`: Input dataset including population, life expectancy, and income metrics.
* `population_growth_line.png`: Time-series visualization of regional trends.
* `population_comparison_bar.png`: Comparative bar chart (2000 vs 2100).

---

**Created as part of the Cisco Data Science Program.**
