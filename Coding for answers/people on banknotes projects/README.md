# 💵 People on Banknotes  
### Exploratory Analysis of Historical Figures Featured on Currency

---

## What the Notebook Actually Does

This notebook performs an **exploratory data analysis of people depicted on banknotes** using the dataset  
`people-on-banknotes.csv`.

Specifically, the notebook:

- Loads the dataset using Pandas
- Inspects the structure and contents of the data
- Analyzes which individuals appear on banknotes
- Examines attributes such as country, role, and historical significance
- Uses grouping and aggregation to summarize representation patterns
- Relies entirely on exploratory analysis and descriptive statistics

The notebook does **not**:
- Build predictive or machine learning models
- Perform statistical hypothesis testing
- Apply natural language processing or network analysis

This is a **clean, descriptive EDA notebook** focused on understanding representation in currency design.

---

## Project Overview

Banknotes often reflect a country’s **history, values, and cultural priorities** by featuring influential individuals.  
This project explores a structured dataset of people shown on banknotes to understand:

- Who is represented
- How representation varies across countries
- Which types of individuals are most commonly featured

The project demonstrates how **cultural and historical data** can be examined using standard data science workflows.

---

## Dataset

**File:** `people-on-banknotes.csv`

Each row in the dataset represents an individual who appears on a banknote.  
The dataset includes attributes such as:

- Person’s name
- Country or currency
- Role or reason for inclusion
- Additional descriptive metadata used for analysis

The dataset is loaded explicitly in the notebook and used throughout the analysis.

---

## Tools & Technologies

- Python
- Pandas
- Matplotlib
- Jupyter Notebook / Google Colab

---

## Analysis Performed

### 1. Data Loading & Inspection
- Loaded `people-on-banknotes.csv` using Pandas
- Examined columns, data types, and sample rows

### 2. Representation Analysis
- Counted how frequently individuals appear
- Examined distribution across countries and regions

### 3. Grouped Aggregation
- Grouped individuals by role or category
- Summarized representation patterns using aggregation functions

### 4. Visualization
- Created basic visualizations to support descriptive findings
- Focused on clarity and interpretability rather than inference

All operations are implemented using standard Pandas methods such as:
- `groupby`
- Aggregation functions
- Sorting and filtering
- DataFrame inspection

---

## Key Observations

- Currency design strongly reflects national identity and historical priorities
- Certain roles (e.g., political leaders, cultural figures) appear more frequently
- Representation varies significantly across countries

All observations are derived directly from notebook outputs.

---

## Repository Structure

```text
├── People on Banknotes.ipynb
├── people-on-banknotes.csv
└── README.md
````

---

## How to Run

### Option 1: Google Colab

1. Upload `People on Banknotes.ipynb` to Google Colab
2. Upload `people-on-banknotes.csv` when prompted
3. Run all cells sequentially

### Option 2: Local Environment

1. Clone the repository
2. Place `people-on-banknotes.csv` in the project directory
3. Open the notebook and run all cells

---

## Project Relevance

This project demonstrates:

* Strong exploratory data analysis fundamentals
* Experience working with cultural and historical datasets
* Ability to extract insights from structured, non-business data
* Clear, reproducible Pandas workflows

It complements other portfolio projects involving:

* Global and geographic data
* Art, design, and perception datasets
* Social and cultural analysis using data

---

## Author

**Bhavik Buchke**
| Data Scientist

---

⭐ This repository is part of a broader, continuously evolving data science portfolio.
