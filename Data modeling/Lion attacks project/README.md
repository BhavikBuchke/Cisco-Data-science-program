# Predator-Prey Dynamics: Analyzing Lion Attacks & Hunger Patterns

## 📋 Executive Summary

This project investigates the environmental and physiological drivers of lion behavior, specifically focusing on human-wildlife conflict and hunting success. By analyzing datasets on lion attacks relative to the lunar cycle and correlating hunger levels with belly size, the study provides a data-driven look at when and why lions are most dangerous to humans. The findings suggest that environmental darkness—specifically the period following a full moon—is a critical predictor of attack frequency.

## ❓ The Problem

Lion attacks on humans in rural Africa are a significant conservation and safety challenge. Understanding the patterns behind these events is essential for developing effective mitigation strategies.

This project explores two core hypotheses:

1. **The Lunar Influence:** Do lions exploit the "period of darkness" in the week following a full moon to hunt humans more effectively?
2. **Hunger Metrics:** Can a lion's hunger level be accurately estimated using a visual "belly size" index?

---

## 🛠️ Technical Workflow

The analysis follows a comprehensive data science methodology:

1. **Data Ingestion & Cleaning:**
* Processed attack records categorized by days since the full moon.
* Cleaned and organized observational data regarding lion belly sizes (ranging from 1 for "very thin" to 5 for "very distended") and estimated hours since their last meal.


2. **Exploratory Data Analysis (EDA):**
* Visualized attack frequencies across the lunar cycle to identify high-risk "danger zones".


3. **Linear Regression Modeling:**
* Developed a predictive model to correlate belly size with hours since eating, providing a quantitative measure for lion hunger.


4. **Causality & Confounding Analysis:**
* Evaluated confounding variables such as seasonality and human behavior (e.g., sleeping outdoors) to contextualize the relationship between darkness and attacks.



---

## 📈 Key Insights & Results

The study highlights a direct link between environmental conditions and predator risk.

| Metric | Analysis Result |
| --- | --- |
| **Peak Attack Period** | **Days 1–10 following a full moon** |
| **Attack Rate Increase** | Attacks are significantly more frequent when the moon rises after sunset. |
| **Hunger Correlation** | Belly size (1-5) serves as a strong inverse proxy for time since last feeding. |

**Core Findings:**

* **The Full Moon Paradox:** While the full moon itself is bright, the evenings immediately following it are the darkest, as the moon rises progressively later. This "window of darkness" sees the highest frequency of lion attacks.
* **Safety Implications:** Data suggests that human vigilance should be highest during the first hour after sunset in the days following a full moon.
* **Visual Hunger Index:** The linear relationship between belly size and time since feeding allows researchers to non-invasively monitor pride nutritional status.

---

## 💻 How to Run

To replicate this analysis:

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data modeling/Lion attacks project"

```


2. **Install Necessary Libraries:**
```bash
pip install pandas matplotlib scipy

```


3. **Run the Notebook:**
Launch `lion attacks.ipynb` in Jupyter or Google Colab. Ensure `lion-attacks-lunar-cycle.csv` and `lion-belly-sizes.csv` are in the project folder.

---

## 🎓 Program Credits

Created as part of the **Cisco Data Science Program**. This project demonstrates the application of statistical modeling to ecology and human-wildlife conflict resolution.

---

**Author:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
