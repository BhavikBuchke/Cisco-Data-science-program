# The Scoville Scale: Visualizing the World's Hottest Peppers

> **Exploring the limits of biological heat through data.**

## 📊 Executive Summary

The Scoville Heat Unit (SHU) is the universal metric for "heat" in chili peppers. While most people are familiar with the spice of a Jalapeño, the world of "Super-Hot" peppers exists on a logarithmic scale of intensity that is difficult to grasp through numbers alone.

This project utilizes Python data visualization to benchmark the top 10 hottest peppers in the world against common household varieties. By creating a comparative visual framework, we illustrate the staggering gap between culinary spice and biological extremes—where the hottest pepper is over **330 times more intense** than a standard Jalapeño.

---

## 🎯 The Business Problem

Communicating abstract, high-magnitude data to a general audience is a core challenge in data storytelling.

* **The Problem:** A value like "2,693,000 SHU" (Pepper X) is impressive but lacks a frame of reference for someone who doesn't study capsaicin.
* **The Goal:** To build a "Benchmark Visualization" that uses a common anchor (the Jalapeño) to make the extreme data points immediately understandable and impactful.

---

## 💡 Key Insights & Results

The analysis of `worlds-hottest-peppers.csv` reveals a tier of "Chemical Weapon" grade peppers that far exceed traditional culinary limits.

| Pepper | Scoville Heat Units (SHU) | Intensity vs. Jalapeño |
| --- | --- | --- |
| **Pepper X** | **2,693,000** | **336x Hotter** |
| **Carolina Reaper** | 2,200,000 | 275x Hotter |
| Trinidad Moruga Scorpion | 2,009,231 | 251x Hotter |
| Ghost Pepper | 1,041,427 | 130x Hotter |
| *Jalapeño (Reference)* | *8,000* | *1x* |

* **The Dominance of Pepper X:** Recently crowned the world's hottest, it sits nearly 500,000 units above the previous record-holder (Carolina Reaper).
* **The "Millionaire" Club:** 9 out of the top 10 peppers in this study exceed 1,000,000 SHU, placing them in an elite category of heat that requires specialized handling.

---

## 🛠 Technical Workflow

### 1. Data Cleaning

The dataset was loaded via `pandas`. The peppers were already ranked by their SHU rating, allowing us to focus directly on the top 10 "Super-Hots."

### 2. Comparative Benchmarking

A "Reference Line" was engineered into the plot at 8,000 SHU. This simple technical addition transforms a standard bar chart into a comparative tool, providing the user with a known baseline for every other data point.

### 3. Visualization Styling

Using `matplotlib`, we implemented several design "Pro Tips":

* **Minimalist Architecture:** Removed all borders (spines) and tick marks to reduce cognitive load.
* **Direct Annotation:** Placed comma-formatted SHU values directly at the end of bars so the audience doesn't have to eye-track back to the axis.
* **Inverted Hierarchy:** Inverted the Y-axis so the #1 hottest pepper occupies the top position, aligning with natural reading patterns.

---

## 📈 Visualizations

### The Scoville Intensity Gap

The horizontal bar chart below highlights the top 10 peppers. Note the red dashed line at the far left—that represents the heat of a standard Jalapeño, effectively invisible compared to the scale of the leaders.

<img width="1000" height="400" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/3554f42f-0906-440d-be2c-ce6f072b6157" />

---

## 🚀 How to Run

To explore the analysis and generate the visualizations locally:

1. **Clone the repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data visualization/Spicy Peppers Project"

```


2. **Install dependencies:**
```bash
pip install pandas matplotlib

```


3. **Launch the Notebook:**
```bash
jupyter notebook "spicy pepper.ipynb"

```



---

## 📂 Project Structure

* `spicy pepper.ipynb`: The primary Python analysis and visualization script.
* `worlds-hottest-peppers.csv`: Dataset containing the top 10 record-holders and their SHU ratings.
* `scoville_analysis.png`: The finalized comparative visualization.

---
**Created as part of the Cisco Data Science Program.**
