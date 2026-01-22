# Flight Delay Analysis: Patterns in Air Travel Logistics

## 📊 Executive Summary

This project investigates the operational patterns of domestic flights departing from the world's busiest airport (Atlanta/ATL) throughout 2023. By analyzing over 5,000 flight records and matching them with national passenger volume data, this study identifies significant correlations between the day of the week and the probability of departure delays.

**Key Finding:** Flight delays are not distributed evenly across the week. **Sunday** emerges as the day with the highest percentage of delays, while **Tuesday** is statistically the most reliable day for on-time departures.

---

## 💼 Business Problem

For airlines and airport authorities, delays represent significant financial losses and decreased customer satisfaction. This analysis addresses three core logistical questions:

1. **Temporal Trends:** Which days of the week consistently face the highest congestion and delay rates?
2. **Operational Benchmarking:** Using the industry standard of a **15-minute grace period**, what is the true "late" rate for a major hub?
3. **Volume vs. Performance:** Does a higher volume of daily passengers across the U.S. directly predict a higher delay rate at individual hubs?

---

## 📈 Key Insights & Results

The analysis revealed a clear "weekend vs. midweek" divide in flight performance:

| Metric | Result |
| --- | --- |
| **Most Delayed Day** | **Sunday** (Highest percentage of flights late by >15 min) |
| **Most Reliable Day** | **Tuesday** (Fewest late flights recorded) |
| **Standard Late Threshold** | **900 Seconds** (15 Minutes) used for binary classification |
| **Passenger Correlation** | Higher passenger volumes typically correspond with increased delay rates. |

---

## 🛠 Technical Workflow

### 1. Data Cleaning & Type Conversion

Raw data for flight schedules was loaded as string objects, which are unsuitable for temporal math.

* **Datetime Parsing:** Converted `scheduled` and `actual` columns into `datetime64` objects using `pd.to_datetime()` to allow for precise arithmetic.

### 2. Feature Engineering

Created custom features to quantify flight performance:

* **Delay Calculation:** Calculated the exact delta between actual and scheduled times.
* **Binary Classification:** Created an `is_late` flag for flights exceeding the 900-second industry delay standard.
* **Temporal Extraction:** Extracted day names (Mon-Sun) to enable day-of-week grouping.

### 3. Data Aggregation & Comparative Analysis

* **Grouping:** Utilized `groupby('day_name')` to calculate the mean of the boolean `is_late` column, representing the proportion of delays per day.
* **External Correlation:** Integrated `us-daily-passengers.csv` to compare local airport performance against national travel demand.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git

```


2. **Navigate to Project Directory:**
`Data cleaning/flights-delays-project/`
3. **Requirements:**
* Python 3.x
* Pandas
* Matplotlib


4. **Execute:**
Open `flight delays.ipynb` in Jupyter or Google Colab and ensure `flights.csv` and `us-daily-passengers.csv` are in the same directory.

---

## 🖼 Visualizations

> **Note:** The notebook generates comparative bar charts for the following:

* **[Percentage of Flights Delayed by Day of Week]:** Highlights the spike in delays during Sunday travel.
* **[Average Daily Passenger Volume]:** Illustrates peak travel days across the United States.

---

**Developed by:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
**Repo Location:** [Cisco Data Science Program](https://www.google.com/search?q=https://github.com/BhavikBuchke/Cisco-Data-science-program/tree/main/Data%2520cleaning/flights-delays-project)

Created as part of the **Cisco Data Science Program**.
