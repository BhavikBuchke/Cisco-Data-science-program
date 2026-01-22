# A Century of Top Songs: Analyzing Hit Song Durations (1923–2023)

## 📊 Executive Summary

This project analyzes the duration of number-one hit songs over a 100-year span, from 1923 to 2023. By transforming raw string data into a quantifiable time-series, this study tracks the evolution of music industry standards. The analysis identifies a significant "duration shift" in the late 1960s and pinpoints the outliers that redefined what constitutes a "radio-friendly" hit.

**Key Finding:** The year **1968** served as a major turning point in music history. The average duration of a top hit increased by over **35%** after this year, moving from roughly 2.9 minutes to 3.9 minutes.

---

## 💼 Business Problem

In the music industry, song duration has historically been dictated by physical media (vinyl records) and radio programming constraints. This analysis addresses:

1. **Ideal Duration:** Is there a statistical "sweet spot" for a chart-topping hit?
2. **Historical Inflection:** When did the industry move away from the "3-minute pop song" standard?
3. **Modern Trends:** Are streaming-era hits (2019–2023) becoming shorter compared to the epic-length hits of the late 20th century?

---

## 📈 Key Insights & Results

| Metric | Result |
| --- | --- |
| **Shortest Top Hit** | **"Sonny Boy" (1928)** — 115 seconds (1m 55s) |
| **Longest Top Hit** | **"Hey Jude" by The Beatles (1968)** — 431 seconds (7m 11s) |
| **Pre-1968 Average** | **173.34 Seconds** (~2.89 minutes) |
| **Post-1968 Average** | **234.33 Seconds** (~3.91 minutes) |

**Trend Analysis:** The data shows a sharp spike in 1968. Following the success of "Hey Jude," the median duration for number-one hits stayed elevated for decades before beginning to fluctuate in the modern streaming era.

---

## 🛠 Technical Workflow

### 1. Data Ingestion & Cleaning

* **Loading:** Imported `top-song-durations.csv` containing 101 years of chart-topping data.
* **Dtype Optimization:** Converted columns to appropriate types using `.convert_dtypes()` to facilitate string operations.

### 2. Feature Engineering

The raw `duration` data was provided as strings (e.g., "00:03:20"), which required transformation for numerical analysis.

* **String Parsing:** Used `.str.split(':')` to isolate hours, minutes, and seconds.
* **Type Casting:** Converted extracted substrings to integers using `.astype('int')`.
* **Unit Conversion:** Calculated a unified `total_seconds` column using the formula:
.

### 3. Exploratory Data Analysis (EDA)

* **Visualization:** Generated a line plot of `total_seconds` vs. `year` to identify outliers and long-term trends.
* **Segmented Analysis:** Compared mean durations of two distinct eras (pre-1968 and post-1968) to quantify the historical shift in song length.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git

```


2. **Navigate to Project:**
`Data cleaning/top songs project/`
3. **Requirements:**
* Python 3.x
* Pandas
* Matplotlib


4. **Run:**
Open `A century of top songs.ipynb` and ensure `top-song-durations.csv` is in the same folder.

---

## 🖼 Visualizations

> **Note:** The notebook generates the following visualization:

* **[Hit Song Duration Over Time]:** A line graph illustrating the 100-year trend, clearly showing the 1968 peak and the subsequent rise in average song length.

---

**Developed by:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)

**Repo Location:** [Cisco Data Science Program](https://www.google.com/search?q=https://github.com/BhavikBuchke/Cisco-Data-science-program/tree/main/Data%2520cleaning/top%2520songs%2520project)

Created as part of the **Cisco Data Science Program**.
