# Aposematism in Nature: Modeling the Link Between Brightness & Toxicity

## 📋 Executive Summary

This project investigates **aposematism**—the biological phenomenon where prey animals use bright coloration as a warning signal to predators. By analyzing data from 10 populations of the Strawberry Poison-Dart Frog (*Oophaga pumilio*), this study applies linear regression to determine if a quantitative link exists between the brightness of a frog's skin and its level of toxicity. The findings provide a statistical basis for understanding how visual signals evolve in tandem with chemical defenses in the wild.

## ❓ The Problem

In evolutionary biology, it is hypothesized that "honest signals" exist where the most conspicuous individuals are also the best defended. However, maintaining high levels of both pigment and poison is metabolically expensive.

This project seeks to answer:

1. **Correlation:** Does higher spectral reflectance (brightness) correlate with higher alkaloid concentration (toxicity)? 


2. **Predictive Modeling:** Can we reliably predict the toxicity of a frog population based solely on visual reflectance data? 



---

## 🛠️ Technical Workflow

The analysis follows a structured data science pipeline:

1. **Data Processing:** * Aggregated spectral reflectance data (measuring how much light the skin reflects) across different frog populations. 


* Combined this with toxicity data (alkaloid concentration) measured from the same populations. 




2. **Object-Oriented Modeling:** * Used a custom `LinearModel` class to perform linear regression, enabling clean code reuse for fitting and plotting. 


3. **Statistical Evaluation:** * Calculated the **Slope** to determine the rate of change in toxicity per unit of brightness. 


* Assessed the **R-squared ()** value to define the strength of the linear relationship. 




4. **Visual Analysis:** * Created scatter plots with regression lines to visualize the "honesty" of the warning signals across different frog populations. 



---

## 📈 Key Insights & Results

The study confirms a strong biological link between visual conspicuousness and chemical defense.

| Metric | Statistical Result |
| --- | --- |
| **Slope** | **11.02** |
| **Intercept** | **-14.73** |
| **R-squared ()** | **0.806** |

**Core Findings:**

* **Positive Correlation:** A slope of ~11.02 indicates that as frogs become brighter, their toxicity levels increase significantly. 


* **Reliable Signals:** An  of **0.81** suggests that approximately 81% of the variation in toxicity can be explained by skin reflectance, supporting the "Honest Signal" hypothesis. 


* **Evolutionary Implications:** The strong linear fit suggests that predators who learn to avoid the brightest frogs are successfully avoiding the most lethal prey, reinforcing the evolution of bright colors. 

---

## 💻 How to Run

To replicate this study:

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data modeling/Poison Dart Frogs Project"

```


2. **Install Dependencies:**
```bash
pip install pandas matplotlib scikit-learn

```


3. **Run the Analysis:**
Launch `poison dart frogs.ipynb` in Jupyter or Google Colab. Ensure `frog-reflectance.csv`, `frog-toxicity.csv`, and `linear_model.py` are present in the working directory. 



---

## 🎓 Program Credits

Created as part of the **Cisco Data Science Program**. This project demonstrates the intersection of data science and evolutionary ecology, using regression to validate biological theories.

---

**Author:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
