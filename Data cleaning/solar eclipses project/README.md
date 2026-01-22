# Solar Eclipse Analysis: Forecasting Celestial Phenomena (1901–2100)

## 📊 Executive Summary

This project explores a century of past and future solar eclipse data, spanning from 1901 to 2100. By processing NASA-level astronomical predictions, the analysis quantifies the duration of total darkness, identifies extreme celestial events, and forecasts upcoming eclipses.

**Key Finding:** The average duration of "Total" solar eclipses is approximately **229 seconds** (~3.8 minutes), providing a benchmark for researchers and eclipse-chasers planning observation missions.

---

## 💼 Business Problem

While solar eclipses are natural phenomena, their predictability is vital for scientific research, telecommunications (ionospheric impact), and tourism logistics. This analysis answers:

1. **Duration Extremes:** When do the longest periods of totality occur for maximum scientific observation?
2. **Type Distribution:** How do "Total," "Annular," and "Partial" eclipses differ in their physical magnitude and duration?
3. **Future Forecasting:** Which regions will host the next major celestial events over the coming decade?

---

## 📈 Key Insights & Results

The analysis extracted specific milestones from the 200-year dataset:

| Metric | Result |
| --- | --- |
| **Longest Solar Eclipse** | Identified based on converted duration in seconds. |
| **Longest Total Eclipse** | Pinpointed as the peak event for researchers. |
| **Average Totality** | **228.93 Seconds** for all Total Solar Eclipses. |
| **Frequency** | Data covers 444 unique events across 200 years. |

---

## 🛠 Technical Workflow

### 1. Data Cleaning

The raw dataset contained gaps and complex string formats:

* **Handling Nulls:** Filtered out partial eclipses that lacked duration data (`NaN`) to ensure accuracy in timing calculations.
* **Precision Filtering:** Focused specifically on the `eclipse_type` categories to prevent skewed averages.

### 2. Feature Engineering (The "Why")

Duration was provided in a human-readable format (e.g., `06m29s`), which is not computable.

* **String Parsing:** Split the `duration` column into `minutes` and `seconds` using string delimiters.
* **Mathematical Conversion:** Calculated total duration in seconds: .
* **Time-Series Alignment:** Converted the `date` column into a `datetime` object to enable chronological sorting and future-dated predictions.

### 3. Quantitative Analysis

* **Querying:** Used `.query()` and boolean indexing to isolate specific types of eclipses and calculate the statistical mean of durations.
* **Forecasting:** Sorted the cleaned dataset by date to identify the "Next 10" upcoming events relative to current time.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git

```


2. **Navigate to Project Directory:**
`Data cleaning/solar eclipses project/`
3. **Dependencies:**
* Python 3.x
* Pandas


4. **Run the Analysis:**
Open `Solar Eclipses.ipynb` in any Jupyter environment and ensure `solar-eclipses.csv` is present in the working directory.

---

## 🖼 Visualizations

> **Note:** The notebook identifies patterns in the following areas:

* **[Duration by Eclipse Type]:** A comparison showing why Annular and Total eclipses are prioritized for research.
* **[Global Reach]:** Analysis of the `region` column showing geographical concentrations of upcoming events.

---

**Developed by:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
**Repo Location:** [Cisco Data Science Program](https://github.com/BhavikBuchke/Cisco-Data-science-program/tree/main/Data%20cleaning/solar%20eclipses%20project)

Created as part of the **Cisco Data Science Program**.
