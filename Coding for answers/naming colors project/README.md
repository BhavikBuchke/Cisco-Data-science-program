# 🎨 Naming Colors  
### Exploratory Analysis of Color Naming Using the Munsell Color System  

---

## What the Notebook Actually Does

This notebook performs an **exploratory data analysis of color naming behavior** using experimental data from the **Munsell color system**.

In the **first code cell**, the notebook includes **Google Colab–specific setup**, where the dataset  
`munsell-array-fixed-choice.csv` is explicitly referenced and loaded.

The notebook:

- Loads `munsell-array-fixed-choice.csv` using Pandas
- Analyzes how participants assign **color names** to standardized color samples
- Works with numeric perceptual color attributes (hue, value, chroma)
- Uses grouping and aggregation to explore naming patterns

The notebook does **not**:
- Train machine learning models
- Perform clustering or prediction
- Conduct statistical hypothesis testing

---

## Project Overview

Color naming is a language-driven process, while the Munsell system provides a structured numeric representation of color perception.  
This project explores how people label colors when presented with controlled color samples, using reproducible data analysis workflows.

---

## Dataset

**File:** `munsell-array-fixed-choice.csv`

Each row represents one color-naming observation and includes:
- Munsell hue, value, and chroma
- The color name selected by participants
- Experimental design intended to minimize ambiguity

The dataset is explicitly referenced in the notebook’s **Google Colab setup cell**.

---

## Tools & Technologies

- Python
- Pandas
- Matplotlib
- Jupyter Notebook / Google Colab

---

## Analysis Performed

### 1. Data Loading
- Dataset loaded using Pandas
- Google Colab compatibility handled in the first code cell

### 2. Naming Frequency Analysis
- Counted occurrences of each color name
- Examined dominance and rarity of labels

### 3. Perceptual Dimension Exploration
- Analyzed how naming varies across hue, value, and chroma
- Used grouping and aggregation for comparison

### 4. Visualization
- Created descriptive plots to support exploratory findings

---

## Key Observations

- Color names correspond to **ranges** in perceptual color space
- Naming boundaries overlap across similar hues
- Structured color systems enable quantitative study of linguistic behavior

All observations are directly supported by notebook outputs.

---

## Repository Structure

```text
├── Naming colors.ipynb
├── munsell-array-fixed-choice.csv
└── README.md
````

---

## How to Run

### Option 1: Google Colab

1. Upload `Naming colors.ipynb` to Google Colab
2. Upload `munsell-array-fixed-choice.csv` when prompted
3. Run all cells sequentially

### Option 2: Local Environment

1. Clone the repository
2. Place `munsell-array-fixed-choice.csv` in the project directory
3. Open the notebook and run all cells

---

## Project Relevance

This project demonstrates:

* Careful, notebook-faithful exploratory data analysis
* Experience working with perceptual and experimental datasets
* Strong Pandas-based grouping and aggregation skills
* Attention to reproducibility and documentation

---

## Author

**Bhavik Buchke**
MCA Student | Data Scientist

---

⭐ This repository is part of a broader, continuously evolving data science portfolio.
