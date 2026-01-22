# Typing Speed Analysis: Identifying Performance Patterns

## 📊 Executive Summary

This project analyzes the results of a typing speed test conducted across a diverse group of participants. By calculating and comparing **Words Per Minute (WPM)** and accuracy rates, the study identifies which typing styles and age groups yield the highest efficiency.

**Key Finding:** The analysis identified the top-performing individual in the dataset, who achieved a typing speed significantly above the group average, providing a benchmark for high-performance typing.

---

## 💼 Business Problem

Understanding human typing efficiency is critical for software design, educational curriculum development, and workplace productivity assessments. This analysis addresses:

1. **Efficiency Benchmarking:** What is the average WPM across different age groups?
2. **Accuracy vs. Speed:** Does a higher typing speed naturally lead to a higher error rate?
3. **Methodological Impact:** Does the participant's typing style (e.g., "hunt and peck" vs. "touch typing") significantly impact their final output?

---

## 📈 Key Insights & Results

The analysis identified clear performance tiers within the test group:

| Metric | Result |
| --- | --- |
| **Top Typing Speed** | Identified as the maximum calculated WPM in the dataset. |
| **Average WPM** | The mean typing speed calculated across all valid test entries. |
| **Accuracy Correlation** | Evaluation of how errors influenced the final net speed calculation. |

---

## 🛠 Technical Workflow

### 1. Data Cleaning & Preparation

The raw dataset required specific preparation to ensure the WPM calculations were based on standardized units:

* **Handling Missing Data:** Identified and addressed any null values within the performance columns.
* **Formatting:** Ensured numerical columns were correctly typed for mathematical operations.

### 2. Feature Engineering

A core component of this project was the creation of a standardized performance metric:

* **WPM Calculation:** Words Per Minute was calculated by dividing total characters by five (the industry standard for a "word") and normalizing for the time taken.
* **Statistical Querying:** Utilized the `.query()` method to isolate top performers and segment the data by age groups.

### 3. Quantitative Analysis

* **Ranking:** Sorted participants by WPM to identify the "fastest" typists.
* **Aggregation:** Used grouping to determine the average performance of specific demographics within the dataset.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git

```


2. **Navigate to Project Directory:**
`Data cleaning/typing speeds project/`
3. **Requirements:**
* Python 3.x
* Pandas


4. **Run the Analysis:**
Open `Typing Speed.ipynb` in your preferred Jupyter environment and ensure `typing-speeds.csv` is in the same directory.

---

## 🖼 Visualizations

> **Note:** The notebook provides data to generate the following insights:

* **[Typing Speed vs. Accuracy]:** Illustrates the relationship between how fast a person types and their error frequency.
* **[WPM by Age Group]:** Shows how typing proficiency varies across different generational cohorts.

---

**Developed by:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
**Repo Location:** [Cisco Data Science Program](https://www.google.com/search?q=https://github.com/BhavikBuchke/Cisco-Data-science-program/tree/main/Data%2520cleaning/typing%2520speeds%2520project)

Created as part of the **Cisco Data Science Program**.
