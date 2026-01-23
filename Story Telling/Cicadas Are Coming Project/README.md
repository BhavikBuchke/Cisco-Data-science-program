# 🦗 The Cicadas are Coming | Decoding the 17-Year Linguistic Heartbeat

---

## 📈 Executive Summary

Periodical cicadas are biological anomalies, emerging from underground in massive, synchronized swarms only once every 13 or 17 years. This project applies data science to historical linguistic records (1700–2019) to uncover the **"cultural heartbeat"** of these insects.

By analyzing word-frequency peaks, we successfully identified the 17-year periodicity in public discourse and pinpointed the specific biological "Broods" (geographic populations) that have historically dominated the English-speaking world's attention.

---

## 🎯 Business & Research Problem

Ecological events often trigger massive spikes in public interest, scientific reporting, and news coverage. For organizations in **environmental communication** or **historical research**, the challenge is identifying which specific recurring events leave the most significant cultural footprint.

This project solves a data-driven "detective" problem: **Can we identify a biological cycle and a specific geographic population using only word-frequency data?**

---

## 💡 Key Insights & Results

The analysis confirmed that human language mirrors biological cycles with remarkable precision.

| Analysis Type | Key Finding | Statistical Context |
| --- | --- | --- |
| **Periodicity** | **17-Year Cycle** | Frequency peaks align with 17-year intervals rather than 13-year cycles. |
| **Dominant Broods** | **Brood II & Brood X** | These two broods account for nearly **2,000 mentions**, significantly outperforming others. |
| **Geographic Inference** | **Urban Correlation** | The prominence of Broods II and X suggests their emergence in regions with higher historical human density. |

### Visualizing the 17-Year Pattern

The chart below illustrates the rhythmic spikes in the usage of the word "cicada." The vertical magenta markers indicate 17-year intervals, aligning almost perfectly with the peaks in literature.

<img width="800" height="400" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/8f2bef8e-2a60-4fce-92df-29e1ea2480c4" />

### The "Celebrity" Broods

By quantifying mentions of specific Roman-numeral broods, we identified which populations drive the most engagement. Brood II and Brood X are the clear leaders in historical prominence.

<img width="800" height="300" alt="Code_Generated_Image(1)" src="https://github.com/user-attachments/assets/686592fa-7771-4fa6-b875-00ac63460616" />

---

## 🛠 Technical Workflow

### 1. Linguistic Pattern Recognition

We utilized a longitudinal dataset of word frequencies (`animal-word-trends-cicada.csv`) to plot the usage of the term "cicada" over a 200-year window.

### 2. Hypothesis Generation (Periodicity)

By measuring the distance between frequency peaks, we formed a hypothesis that **17-year cicadas** generate significantly more cultural impact than their 13-year counterparts.

### 3. Brood Correlation

We overlaid historical emergence dates for the four largest 17-year broods (X, XIV, II, and IV) onto the word-frequency timeline to observe which populations "claimed" the biggest spikes.

### 4. Verification with Print Data

To validate the visual findings, we analyzed a second dataset (`cicada-brood-mentions-print.csv`) containing total mention counts from 1915 to 1970 to confirm which broods were objectively the most "famous."

---

## 🚀 How to Run

To replicate the analysis:

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Story Telling/Cicadas Are Coming Project"

```


2. **Install Dependencies:**
```bash
pip install pandas matplotlib

```


3. **Open the Notebook:**
Launch `cicadas are coming.ipynb` in Jupyter or VS Code.
4. **Dataset Requirements:**
The notebook requires `animal-word-trends-cicada.csv` and `cicada-brood-mentions-print.csv` in the same directory.

---

### 🧰 Tech Stack

* **Language:** Python
* **Libraries:** Pandas (Data Processing), Matplotlib (Time-Series Visualization)
* **Concept:** Periodic Trend Analysis & Correlation Studies

---

*Created as part of the **Cisco Data Science Program**.*
