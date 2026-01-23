# 🪸 Coral Conundrum | Investigating the 1998 Linguistic Collapse

---

## 📈 Executive Summary

In the late 1990s, the linguistic footprint of coral reef fish in printed literature underwent a dramatic and sudden decline. This project investigates this "Coral Conundrum" by analyzing word frequency data alongside ecological and technological milestones.

By correlating species diversity in printed identification guides with cultural mentions, we demonstrate that the rise of the internet—exemplified by the launch of Google and FishBase in 1998—triggered a shift from printed records to digital platforms, fundamentally changing how we document and discuss marine biodiversity.

---

## 🎯 Business & Research Problem

How do we distinguish between an ecological disaster and a technological shift? A sharp drop in the mention of "Coral Reef Fish" could signal a mass extinction event (the "Why" of ecology) or a change in where humans record information (the "Why" of data science).

This project uses **Linear Regression** and **Time-Series Analysis** to determine if the 1998 drop was caused by:

1. **Ecological Stress:** Major global coral bleaching events.
2. **Technological Disruption:** The transition from printed guidebooks to digital search engines.

---

## 💡 Key Insights & Results

The data suggests a "perfect storm" of events in 1998, with the **Internet Effect** being the most likely driver of the decline in *printed* word frequency.

| Metric | Result | Insight |
| --- | --- | --- |
| **Linear Correlation (R²)** | **0.657** | 66% of a fish's literary prominence was historically driven by its diversity in printed guides. |
| **Ecological Peak** | **1998 Bleaching** | A massive spike in global bleaching events coincided with the linguistic drop. |
| **Media Shift** | **Digital Migration** | The founding of Google (1998) and FishBase (1998) created a "digital drain" on printed literature. |

### Visual 1: The 1998 "Drop"

Most coral reef species, such as the Butterflyfish, show a significant and sustained decline in printed frequency starting exactly in 1998.
<img width="800" height="300" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/4f0c1860-468b-4b2a-892a-ca9bb1e84508" />


### Visual 2: The Power of the Printed Guide

Our linear model proves that before the internet, "richer" fish families in identification guides dominated the cultural conversation. As these guides were replaced by digital search, the "anchor" for these word frequencies in the Google Books corpus was removed.

<img width="800" height="350" alt="Code_Generated_Image(2)" src="https://github.com/user-attachments/assets/b79e4a3c-23dd-487d-a95a-79f15550c26c" />
<img width="800" height="300" alt="Code_Generated_Image(1)" src="https://github.com/user-attachments/assets/8b031272-cdfe-4fee-8e34-44efcca38a28" />

---

## 🛠 Technical Workflow

### 1. Exploratory Data Analysis (EDA)

Identified the 1998 inflection point across dozens of reef fish species using the `animal-word-trends-coral-conundrum.csv` dataset.

### 2. Ecological Correlation

Analyzed `bleaching-reefs.csv` and `global-coral-cover.csv` to see if the decline mirrored physical reef loss. While 1998 was a record year for bleaching, the linguistic drop was more permanent than the ecological recovery periods.

### 3. Predictive Modeling (Linear Regression)

* **Feature Engineering:** Merged word frequency data with data from "Reef Fish Identification" guides.
* **Modeling:** Built a linear model (using a custom `LinearModel` class) to quantify how much of a fish's "fame" was tied to its presence in printed books.
* **Validation:** Achieved an R-squared value of **0.66**, confirming that printed guides were major drivers of terminology in the pre-internet era.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Story Telling/Coral Conundrum Project"

```


2. **Install Dependencies:**
```bash
pip install pandas matplotlib scikit-learn

```


3. **Run the Analysis:**
Open `coral conundrum.ipynb` in your preferred Jupyter environment. Ensure `linear_model.py` and all CSV files are in the working directory.

---

### 🧰 Tech Stack

* **Language:** Python
* **ML Library:** Scikit-Learn (Linear Regression)
* **Visualization:** Matplotlib
* **Data Handling:** Pandas

---

*Created as part of the **Cisco Data Science Program**.*
