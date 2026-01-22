# Wildlife Conservation Analysis: Modeling Elephant Tusk Development

## 📋 Executive Summary

This project investigates the biological growth patterns of African elephants, specifically focusing on the relationship between physical maturity and tusk size. By applying linear regression analysis to data from male elephants, this study provides a mathematical framework for predicting an elephant's age based on tusk measurements. Such models are vital for conservation efforts, population health monitoring, and identifying individuals targeted by illegal poaching.

## ❓ The Problem

In wildlife conservation, determining the age of an elephant is essential for understanding population dynamics and reproductive health. However, performing physical age assessments in the wild is difficult and dangerous.

This project seeks to:

1. **Quantify Growth:** Establish the mathematical relationship between a male elephant's age (years) and the length of its tusks (cm).
2. **Predictive Accuracy:** Determine how much of an elephant's physical development can be accurately explained by age alone versus other environmental factors.

---

## 🛠️ Technical Workflow

The analysis followed a professional data science pipeline:

1. **Data Ingestion:**
* Processed historical data for male elephants, including recorded age and corresponding tusk length.




2. **Object-Oriented Modeling:**
* Utilized a custom `LinearModel` class (leveraging `scikit-learn`) to maintain a clean, reusable architecture for the regression analysis.




3. **Statistical Modeling:**
* Fitted a **Linear Regression** model to the data to identify the "line of best fit" for elephant growth.




4. **Performance Evaluation:**
* Extracted the **Slope**, **Intercept**, and **R-squared ()** values to validate the model's reliability.





---

## 📈 Key Insights & Results

The analysis confirms that tusk size is a powerful indicator of biological age in male elephants.

| Metric | Statistical Result |
| --- | --- |
| **Slope** | <br>**5.41** |
| **Intercept** | <br>**44.91**  |
| **R-squared ()** | <br>**0.84**  |

**Core Findings:**

* **Predictive Growth:** A slope of **5.41** suggests that, on average, a male elephant's tusks grow by approximately 5.4 cm per year.


* **High Correlation:** An  value of **0.84** indicates that age explains 84% of the variation in tusk size. This demonstrates that tusk length is a highly reliable metric for non-invasive age estimation in the field.


* **Biological Starting Point:** The intercept of **44.91** represents the modeled baseline length as the elephant matures toward its recorded growth stages.

---

## 💻 How to Run

To replicate this study:

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data modeling/Tusked elephant project"

```


2. **Install Dependencies:**
```bash
pip install pandas matplotlib scikit-learn

```


3. **Run the Analysis:**
Open `tusked elephants.ipynb` in your preferred Jupyter environment. Ensure `male-elephant-tusk-size.csv` and `linear_model.py` are in the same directory.



---

## 🎓 Program Credits

Created as part of the **Cisco Data Science Program**. This project demonstrates the practical application of regression modeling to solve complex biological and conservation challenges.

---

**Author:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
