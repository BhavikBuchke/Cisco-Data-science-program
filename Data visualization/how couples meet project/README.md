# How Couples Meet: The Impact of the Internet on Modern Romance

> **Exploring how technology connects us, one couple at a time.**

## 📊 Executive Summary

The way humans find romantic partners has undergone a seismic shift over the last half-century. This project analyzes the evolution of dating from 1960 to 2010, specifically investigating how the rise of the internet has disrupted traditional social structures like "meeting through friends" or "at work."

Using historical survey data, we visualize the decline of physical social proximity and the explosive growth of digital matching. The results reveal that by 2010, the internet became the most common way for couples to connect, fundamentally changing the landscape of human relationships.

---

## 🎯 The Business Problem

Social connectivity is at the heart of networking and technology. For a company like **Cisco**, which was founded on the need for two people to connect across a distance, understanding how technology facilitates human connection is vital.

* **The Problem:** Traditional methods of meeting—through friends, family, or the workplace—are in decline.
* **The Goal:** To quantify the "Digital Revolution of Romance" and visualize which social channels are being replaced by online platforms.

---

## 💡 Key Insights & Results

The analysis shows a dramatic restructuring of social dynamics between 1960 and 2010:

| Meeting Method | Trend (1960 vs. 2010) | Insight |
| --- | --- | --- |
| **Online** | **0%  42%** | From non-existent to the #1 most common meeting method. |
| **Friends** | 46%  29% | Sharp decline; social circles are becoming less central to matchmaking. |
| **Family** | 30%  10% | Massive decline; the "family introduction" is becoming a rarity. |
| **At Work** | 18%  15% | Relatively stable but overshadowed by more efficient digital alternatives. |

* **The Tipping Point:** Around the late 1990s, "Online" dating began its exponential climb, coinciding with the mass adoption of the internet.
* **The Displacement Effect:** As digital connectivity rose, "Through Family" and "Through Friends" saw the most significant losses in share, suggesting that people are stepping outside their immediate physical social bubbles.

---

## 🛠 Technical Workflow

### 1. Data Cleaning & Transformation

The project utilizes `how-couples-met.csv`, which provides the percentage of couples who met through various methods by decade.

* **Indexing:** The `decade` column was set as the index to facilitate time-series plotting.
* **Normalization:** Data was processed to ensure clear percentage comparisons across decades.

### 2. High-Impact Visualization (The "Focus" Method)

To make the data "Recruiter-Ready," we implemented several advanced Matplotlib techniques:

* **The "Background/Foreground" Strategy:** Traditional methods are plotted in muted colors with low alpha transparency, while the primary focus (**Online**) is highlighted in a bold, thick red line.
* **Direct Labeling:** Instead of a complex legend, category names are placed directly at the end of the lines for instant readability.
* **Clean Axes:** Removed top and right spines and softened the grid to emphasize the trend lines.

### 3. Comparative Analysis

Generated categorical bar charts comparing specific decades (e.g., 1980 vs. 2000) to provide a snapshot of social change before and after the internet's widespread emergence.

---

## 📈 Visualizations

### 1. The Digital Revolution (1960 - 2010)

This line chart shows the meteoric rise of online dating relative to all other social channels. Note how the red line (Online) crosses over traditional methods starting in the mid-90s.

<img width="800" height="400" alt="Code_Generated_Image(1)" src="https://github.com/user-attachments/assets/4ad684da-ff24-4ef7-b02a-1529a4a788a8" />


### 2. Comparative Snapshots: 1980 vs. 2000

Comparing these two decades highlights the "before and after" of the internet era. By 2000, "Online" had already begun to climb the ranks of popularity.

<img width="800" height="600" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/6440aaf6-29be-46de-bf61-415cb30d896c" />

---

## 🚀 How to Run

To explore the analysis and generate the visualizations locally:

1. **Clone the repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data visualization/how couples meet project"

```


2. **Install dependencies:**
```bash
pip install pandas matplotlib

```


3. **Launch the Notebook:**
```bash
jupyter notebook "the internet and dating.ipynb"

```



---

## 📂 Project Structure

* `the internet and dating.ipynb`: The main analytical notebook containing Python code and visualization logic.
* `how-couples-met.csv`: The primary dataset covering dating trends across six decades.
* `rise_of_online_dating.png`: Time-series trend visualization.
* `meeting_methods_comparison.png`: Snapshot bar charts for decade comparisons.

---

**Created as part of the Cisco Data Science Program.**
