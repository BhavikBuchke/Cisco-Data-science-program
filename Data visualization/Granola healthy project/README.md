# The Health Perception Gap: Public vs. Experts

> **Bridging the gap between marketing and nutrition.**

## 📊 Executive Summary

What we believe is healthy often differs from what nutritional science tells us. This project analyzes the divergence between public opinion and expert consensus regarding the healthiness of common foods. By visualizing survey data from both groups, we identify "Marketing Traps" (foods the public overrates) and "Hidden Superfoods" (foods the public underrates).

The core of this project is a **Consensus Matrix**, which uses paired scatter plots to pinpoint exactly where public education on nutrition is succeeding—and where it is failing.

---

## 🎯 The Business Problem

Food manufacturers often use "Health Halos" to market products. This creates a disconnect between perceived health benefits and actual nutritional value.

* **The Problem:** When the public significantly overestimates a food's healthiness (e.g., Granola), it leads to suboptimal dietary choices despite "healthy" intentions.
* **The Goal:** To quantify this perception gap and identify the specific foods where the discrepancy is most extreme.

---

## 💡 Key Insights & Results

The analysis identified four distinct categories of food based on opinion alignment:

| Category | Typical Foods | Impact |
| --- | --- | --- |
| **Public Overestimates** | **Granola Bars**, **Coconut Oil**, Frozen Yogurt | Marketing has successfully convinced the public these are "health foods" despite expert skepticism. |
| **Experts Favor** | **Quinoa**, **Tofu**, Hummus, Sushi | These are nutritionally dense foods that have not yet achieved full mainstream public "health status." |
| **High Consensus (Healthy)** | **Apples**, Almonds, Oatmeal | Universal agreement on their nutritional value. |
| **High Consensus (Unhealthy)** | **Diet Soda**, French Fries, Cookies | Success in public health messaging regarding processed/sugary foods. |

### The "Disagreement" Leaders

* **Granola Bars:** 70% of the public considers them healthy, while only **28% of experts** agree—a staggering **42% gap**.
* **Quinoa:** Only 58% of the public identifies it as healthy compared to **89% of experts**.

---

## 🛠 Technical Workflow

### 1. Data Cleaning & Normalization

The project processes two separate datasets (`healthy-food-survey-public.csv` and `healthy-food-survey-experts.csv`). We calculate a "Healthiness Score" by normalizing the "Yes" votes against the total number of survey participants (Yes + No + No Opinion).

### 2. Data Integration

Datasets were merged into a master frame using the food name as the primary key. This allowed for the calculation of the `difference` metric used to categorize the foods.

### 3. Visualization Engineering

The project utilizes a specialized **Paired Scatter Plot** with several "Pro Tips":

* **The Equality Line:** A dashed  line allows for instant visual identification of who favors a food more.
* **Categorical Coloring:** Points are colored by their consensus status (e.g., "Public considers healthier").
* **Smart Labeling:** To maintain clarity, only extreme outliers and representative consensus foods are labeled.
* **Aspect Ratio:** A strictly square 1:1 aspect ratio is used to prevent visual bias in the slope of the data.

---

## 📈 Visualizations

### The Consensus Matrix

In the plot below, the further a point is from the diagonal line, the greater the disagreement between the public and nutrition experts.

<img width="800" height="800" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/1c7ccdf1-379d-43cc-a9be-6bf7e526d666" />

---

## 🚀 How to Run

To explore the analysis and generate the visualizations locally:

1. **Clone the repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data visualization/Granola healthy project"

```


2. **Install dependencies:**
```bash
pip install pandas matplotlib

```


3. **Launch the Notebook:**
```bash
jupyter notebook "is garnola healthy.ipynb"

```



---

## 📂 Project Structure

* `is garnola healthy.ipynb`: The primary analysis and visualization notebook.
* `healthy-food-survey-public.csv`: Survey data from the general public.
* `healthy-food-survey-experts.csv`: Survey data from nutrition experts.
* `health_perception_gap.png`: The final analytical visualization.

---
**Created as part of the Cisco Data Science Program.**
