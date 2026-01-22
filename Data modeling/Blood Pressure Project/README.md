# Blood Pressure & Aging: A Comparative Data Study

## 📋 Executive Summary

This project investigates a fundamental health question: **Is the increase in blood pressure an inevitable part of biological aging?** By applying linear regression analysis to two distinct populations—modern Americans and the isolated Yanomami tribe of the Amazon—this study reveals how lifestyle factors, specifically sodium intake, potentially influence cardiovascular health trajectories.

## ❓ The Problem

In modern industrial societies, systolic blood pressure (SBP) typically rises as individuals age, leading to high rates of hypertension. However, it is unclear if this is a "natural" biological process.

This study compares:

1. **US Population:** Average sodium intake of **~3,500 mg/day**.
2. **Yanomami Tribe:** Isolated hunter-gatherers with an intake of **<100 mg/day**.

The goal is to model the relationship between age and blood pressure in both groups to determine if aging leads to hypertension in the absence of high-sodium, processed diets.

---

## 🛠️ Technical Workflow

The analysis followed a structured data science pipeline:

1. **Data Preparation:** * Cleaned and processed datasets for the US (NHANES survey) and the Yanomami people.
* Feature Engineering: Calculated the `avg_bp` for the US dataset by averaging three separate readings per participant to ensure data reliability.


2. **Object-Oriented Modeling:** * Utilized a custom `LinearModel` class (built on `scikit-learn`) to encapsulate the fitting, prediction, and visualization logic.
3. **Statistical Analysis:** * Performed Linear Regression to find the best-fit lines for both populations.
* Evaluated model performance using **R-squared ()** values.


4. **Visualization:** * Generated side-by-side scatter plots and regression lines to visualize the contrast in aging trajectories.

---

## 📈 Key Insights & Results

The disparity between the two populations is stark and provides significant evidence for the impact of environmental factors on health.

| Metric | US Population (High Sodium) | Yanomami Tribe (Low Sodium) |
| --- | --- | --- |
| **Slope (Growth Rate)** | **0.74** | **-0.004** |
| **Predictive Power ()** | 0.47 | 0.00005 |
| **Observation** | BP increases ~0.75 mmHg per year. | BP remains stable throughout life. |

### Visual Comparison

**Core Conclusions:**

* **Aging  Hypertension:** The Yanomami model shows a slope of near-zero, proving that blood pressure does not have to increase with age.
* **Environmental Impact:** The moderate  in the US (0.47) suggests age is a strong predictor of BP in modern environments, whereas, in the Yanomami environment, age has zero predictive power over cardiovascular health.

---

## 💻 How to Run

To replicate this study on your local machine:

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data modeling/Blood Pressure Project"

```


2. **Install Dependencies:**
Ensure you have Python installed, then run:
```bash
pip install pandas matplotlib scikit-learn

```


3. **Run the Notebook:**
Launch Jupyter Notebook or open the `.ipynb` file in VS Code/Google Colab and run all cells. Note that `linear_model.py` must be in the same directory as the notebook.

---

## 🎓 Program Credits

Created as part of the **Cisco Data Science Program**. This project demonstrates proficiency in exploratory data analysis (EDA), predictive modeling, and the ability to derive actionable health insights from complex datasets.

---

**Author:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
