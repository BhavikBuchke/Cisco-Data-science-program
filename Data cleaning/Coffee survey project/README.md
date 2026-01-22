# Plant-Based Coffee Shop Strategy: A Data-Driven Approach

This repository contains a data analysis project focused on optimizing the product offerings for a new specialty coffee shop specializing in plant-based beverages. By leveraging survey data from over 1,000 coffee enthusiasts, this analysis identifies consumer dairy preferences to ensure inventory aligns with market demand.

---

### ☕ Executive Summary

The objective of this project is to provide actionable recommendations for a plant-based coffee shop's inventory. Using a dataset of approximately 1,170 respondents, the analysis focuses on isolating the preferences of coffee drinkers who use dairy or dairy alternatives.

**Key Result:** Among specialty coffee enthusiasts, **Oat milk** is the definitive leader in the plant-based market, preferred by nearly **39% of respondents**. While traditional whole milk remains the overall most popular choice, the high demand for oat milk suggests it should be the primary offering for any plant-based specialty establishment.

---

### ❓ The Problem

Specialty coffee shops operate in a highly competitive market where inventory decisions impact both customer satisfaction and waste management. For a shop moving toward a plant-based model, it is critical to know: **"Which dairy alternatives are preferred by specialty coffee enthusiasts?"** and **"Which options will capture the largest possible segment of the traditional dairy-drinking audience?"**

---

### 📈 Key Insights & Results

The analysis of 523 dairy-using respondents revealed a clear hierarchy of preferences:

| Dairy/Alternative Type | Preference Percentage |
| --- | --- |
| **Whole milk** | **56.2%** |
| **Oat milk** | **38.8%** |
| Half and half | 23.3% |
| Almond milk | 10.3% |
| Flavored creamer | 9.4% |
| Skim milk | 7.1% |
| Coffee creamer | 6.7% |
| **Soy milk** | **5.7%** |

*Note: Respondents could select multiple preferences, so total percentages exceed 100%.*

#### Visualization: Dairy Preference Distribution

> **Strategic Recommendation:** Focus heavily on **Oat milk** as the default plant-based alternative. While almond and soy milk are industry standards, their significantly lower preference rates (10.3% and 5.7% respectively) suggest they should be secondary offerings.

---

### 🛠 Technical Workflow

The analysis follows a clean, reproducible pipeline designed for clarity and accuracy:

1. **Data Acquisition**: Survey data was loaded from `coffee-survey-results.csv` using `pandas`.
2. **Feature Selection**: The original dataset contained 30 complex columns; the analysis isolated the 8 columns specifically related to dairy consumption types.
3. **Data Cleaning**:
* **Header Renaming**: Verbose question-based headers (e.g., *"What kind of dairy? (Whole milk)"*) were mapped to simple labels like *"Whole milk"* to improve code readability and visualization aesthetics.
* **Handling Missing Values**: 647 respondents were removed from the specific dairy analysis because they indicated they did not use dairy (drinking black coffee), ensuring the final ratios accurately reflected only dairy users.


4. **Exploratory Data Analysis (EDA)**: The `mean()` method was used to calculate the frequency of each dairy choice, converted into a percentage for comparison.
5. **Visualization**: Data was sorted and visualized using `matplotlib` to create a horizontal bar chart for high-impact communication of the results.

---

### 📂 Repository Structure

* `A plant based coffee shop.ipynb`: The primary Jupyter Notebook containing the data cleaning and analysis.
* `coffee-survey-results.csv`: The initial dataset used for analysis.
* `coffee-survey-full-dataset.csv`: An expanded dataset containing 113 columns for extended research (e.g., demographic analysis, brewing methods).

---

### 🚀 How to Run

1. **Clone the Repository**:
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data cleaning/Coffee survey project"

```


2. **Environment Setup**:
Ensure you have Python installed. Install the necessary libraries:
```bash
pip install pandas matplotlib

```


3. **Execution**:
Open `A plant based coffee shop.ipynb` in your preferred editor (Jupyter, VS Code, or Google Colab) and run all cells to reproduce the findings and visualizations.

---

*Created as part of the Cisco Data Science Program.*
