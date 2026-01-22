# Lion Age Prediction via Nose Pigmentation: Data Study

## 📋 Executive Summary

This project explores a non-invasive biological marker for wildlife conservation: **Can the age of a male lion be accurately predicted by the amount of black pigmentation on its nose?** Using linear regression, this study demonstrates a strong correlation between age and nose color, providing conservationists with a mathematical tool to estimate lion ages without risky physical examinations.

## ❓ The Problem

In wildlife management, knowing the age of a lion is crucial for pride management and sustainable trophy hunting (which typically requires lions to be over 6 years old). Traditional methods of aging—such as tooth wear or mane development—can be subjective or require sedation.

This project analyzes data from **32 male lions** of known age to:

1. Quantify the relationship between age and the proportion of black nose pigmentation.


2. Develop a predictive model to estimate age based on a simple visual metric.

---

## 🛠️ Technical Workflow

The analysis followed a rigorous data modeling process:

1. 
**Data Acquisition:** * Processed a dataset of 32 lions, measuring age (years) and nose pigmentation (proportion of black).


2. **Object-Oriented Modeling:**
* Employed a custom `LinearModel` class built on top of `scikit-learn` to manage the fitting, prediction, and extraction of statistical metrics.




3. **Statistical Validation:**
* Calculated **Slope** and **Intercept** to define the linear relationship.


* Evaluated the **R-squared ()** value to measure the reliability of the prediction.




4. **Visualization:**
* Created scatter plots overlaid with the regression model to visualize how closely nose color tracks with biological aging.



---

## 📈 Key Insights & Results

The analysis reveals that nose pigmentation is a highly effective "biological clock" for male lions.

| Metric | Statistical Result |
| --- | --- |
| **Slope** | **10.65** |
| **Intercept** | **0.88** |
| **R-squared ()** | **0.938** |

---

**Key Findings:**

* 
**Strong Correlation:** An  of **~0.94** indicates that nearly 94% of the variation in a lion's age can be explained by nose pigmentation.


* **Predictive Accuracy:** With a slope of 10.65, the model suggests that for every 0.1 increase in the proportion of black on the nose, a lion is roughly one year older.
* **Practical Application:** This high degree of accuracy supports the use of nose color as a primary non-invasive age-estimation technique in the field.

---

## 💻 How to Run

To run this project locally:

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data modeling/Lion Nose Color Project"

```


2. **Install Requirements:**
```bash
pip install pandas matplotlib scikit-learn

```


3. **Execute the Analysis:**
Open `lion nose color.ipynb` in your preferred Jupyter environment. Ensure `linear_model.py` and `lion-nose-color.csv` are in the same directory.

---

## 🎓 Program Credits

Created as part of the **Cisco Data Science Program**. This project exemplifies the use of regression analysis to solve real-world biological and conservation challenges through data.

---

**Author:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
