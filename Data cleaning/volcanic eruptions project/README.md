# Global Volcanic Activity: Analysis of Historical Eruption Durations (1800–2024)

## 📊 Executive Summary

This project examines a comprehensive catalog of over **3,700 volcanic eruptions** since the year 1800. By integrating eruption event logs with a master list of global volcanoes, this analysis identifies the most active geological sites and quantifies the duration of historic eruptions.

**Key Finding:** The analysis identified extreme geological events where eruptions spanned over **90 years**, highlighting the persistent nature of specific volcanic systems.

---

## 💼 Business Problem

Volcanic monitoring is essential for disaster preparedness, aviation safety, and climate modeling. This analysis provides data-driven answers to:

1. **Duration Extremes:** Which volcanoes sustain the longest active eruptions, and what are their primary types?
2. **Ongoing Risks:** As of late 2024, which volcanoes are currently in an active state?
3. **Geographic Distribution:** Which countries and tectonic settings are home to the most frequently erupting systems?

---

## 📈 Key Insights & Results

The study processed data from over 1,200 unique volcanoes to find these patterns:

| Metric | Result |
| --- | --- |
| **Longest Eruption Observed** | **94 Years** (Identified in the duration analysis) |
| **Total Events Analyzed** | **3,724** Eruptions since 1800 |
| **Active Monitoring** | List of volcanoes currently erupting as of **Dec 2024** |
| **Primary Tectonic Settings** | Correlation between eruption frequency and subduction/rift zones. |

---

## 🛠 Technical Workflow

### 1. Data Cleaning & Integration

* **Dataset Merging:** Performed a relational `merge` between `volcanic-eruptions.csv` and `volcano-list.csv` using the `volcano_id` as the primary key.
* **Column Reduction:** Removed metadata columns (e.g., `volcanic_region`, `dominant_rock_type`) to focus strictly on temporal and geographic variables.

### 2. Feature Engineering

Raw date strings were transformed to enable duration math:

* **Datetime Conversion:** Converted `start_date` and `end_date` into `datetime64` objects.
* **Temporal Math:** Extracted years from the datetime objects to calculate the `duration_in_years` for every event.
* **Filtering:** Used `.query()` to isolate "currently active" volcanoes based on the December 2024 timestamp.

### 3. Exploratory Data Analysis (EDA)

* **Ranking:** Sorted the merged dataset to identify the top 5 longest eruptions in modern history.
* **Current Status Report:** Generated a specific slice of the data representing ongoing eruptions to assist in "real-time" status reporting.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git

```


2. **Navigate to Project Directory:**
`Data cleaning/volcanic eruptions project/`
3. **Requirements:**
* Python 3.x
* Pandas


4. **Run:**
Open `Volcanic Eruption.ipynb` in a Jupyter environment. Ensure both `volcanic-eruptions.csv` and `volcano-list.csv` are in the working directory.

---

## 🖼 Visualizations

> **Note:** The analysis provides data for the following:

* **[Histogram of Eruption Durations]:** Shows that while most eruptions are short, a significant few last for decades.
* **[Global Activity Heatmap]:** Using the provided `latitude` and `longitude` coordinates from the master list.

---

**Developed by:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
**Repo Location:** [Cisco Data Science Program](https://www.google.com/search?q=https://github.com/BhavikBuchke/Cisco-Data-science-program/tree/main/Data%2520cleaning/volcanic%2520eruptions%2520project)

Created as part of the **Cisco Data Science Program**.
