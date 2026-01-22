# Blue Whale Heart Rate Analysis: Physiological Dynamics During Deep Foraging

## 📊 Executive Summary

This project investigates the extreme physiological adaptations of blue whales during deep-sea foraging dives exceeding 100 meters. By analyzing high-frequency heart rate telemetry data across various dive phases—Descent, Lunging, Filtering, Ascent, and Surface—this study quantifies how a whale's cardiovascular system responds to extreme pressure and physical exertion.

**Key Finding:** The analysis establishes a direct correlation between **dive duration** and the **maximum surface heart rate** following the event, providing insight into the "oxygen debt" recovery process of the world's largest mammal.

---

## 💼 Business & Scientific Problem

Understanding the metabolic limits of endangered species is critical for conservation efforts and marine biology research. This analysis addresses:

1. **Phase-Based Heart Rate Variance:** How significantly does the heart rate drop during the descent versus the active "lunging" phase?.
2. **Metabolic Recovery:** How does the duration of a deep dive affect the heart's recovery rate once the whale returns to the surface?.
3. **Efficiency Modeling:** Quantifying the "Filtering" phase to understand the energy cost of processing prey.

---

## 📈 Key Insights & Results

The analysis identified distinct cardiovascular markers for each phase of the foraging dive:

| Dive Phase | Physiological Description |
| --- | --- |
| **Descent** | Cardiovascular slowing to conserve oxygen during the dive start. |
| **Lunging** | High-exertion spikes as the whale engulfs massive amounts of water and prey. |
| **Filtering** | Slight heart rate stabilization while water is expelled. |
| **Ascent** | Gradual increase in heart rate during the return to the surface. |
| **Surface** | Peak heart rates (recovery phase) to replenish oxygen stores. |

---

## 🛠 Technical Workflow

### 1. Data Cleaning & Standardization

* **Handling Irregularities:** Removed incomplete records using `.dropna()` to ensure statistical integrity.
* **Time-Series Parsing:** Converted `timestamp` strings into `datetime` objects to allow for precise duration calculations.

### 2. Feature Engineering

Created complex secondary metrics to analyze physiological recovery:

* **Dive Duration Calculation:** Aggregated timestamps to find the delta between the first `descent` marker and the final `ascent` marker for each unique `dive_id`.
* **Recovery Peak Isolation:** Filtered surface-level data (top 5 meters) to identify the absolute maximum heart rate achieved during post-dive breathing.
* **Relational Merging:** Unified duration and recovery data into a master dataframe to enable correlation testing.

### 3. Quantitative Analysis & Visualization

* **Descriptive Statistics:** Calculated the average heart rate per phase using `groupby` operations.
* **Scatter Analysis:** Utilized `matplotlib` to plot **Dive Duration vs. Max Surface Heart Rate**, identifying the relationship between underwater time and cardiovascular recovery demand.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git

```


2. **Navigate to Project Directory:**
`Data cleaning/whale heart rates project/`
3. **Requirements:**
* Python 3.x
* Pandas
* Matplotlib


4. **Run:**
Execute `Whale Heart rate.ipynb` in any Jupyter or Google Colab environment. Ensure `blue-whale-heart-rates.csv` is uploaded.

---

**Developed by:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
**Repo Location:** [Cisco Data Science Program](https://github.com/BhavikBuchke/Cisco-Data-science-program/tree/main/Data%20cleaning/whale%20heart%20rates%20project)

Created as part of the **Cisco Data Science Program**.

---

Would you like me to help you draft a cover letter or a LinkedIn post highlighting these specific data science projects for your portfolio?
