# Emoji Sentiment Analysis: Decoding Digital Emotion

## 📊 Executive Summary

This project analyzes a dataset of **1.6 million tweets** across 13 European languages to determine the sentiment patterns of popular emojis. By calculating a custom sentiment score and applying data cleaning techniques, this study quantifies how digital icons correlate with positive, negative, and neutral human emotions.

**Key Finding:** Over **82%** of emojis in the dataset are associated with positive sentiments, suggesting that emojis serve primarily as tools for positive reinforcement in digital communication.

---

## 💼 Business Problem

In the field of Natural Language Processing (NLP), understanding the "contextual weight" of an emoji is critical for sentiment analysis. Brands and researchers often struggle with:

1. **Sentiment Ambiguity:** Does a specific emoji skew a message's intent?
2. **Model Accuracy:** Can we improve automated customer service tools by weighing emoji sentiment?
3. **Communication Trends:** Where do users naturally place emotional markers within a message?

This project provides a prototype for bucketing and scoring these digital assets to improve brand perception monitoring and social listening tools.

---

## 📈 Key Insights & Results

The analysis yielded the following high-impact data points:

| Metric | Result |
| --- | --- |
| **Global Sentiment Bias** | **82.29%** of all emojis in the dataset carry a positive sentiment. |
| **Popular Emoji Sentiment** | **78.40%** of the Top 20 most frequently used emojis are positive. |
| **Average Placement** | Emojis appear at an average position of **0.67** (approx. 2/3 through a tweet). |
| **Most Positive (>500 mentions)** | Heavy Black Heart (🖤) |
| **Most Negative (>500 mentions)** | Broken Heart (💔) |

---

## 🛠 Technical Workflow

### 1. Data Cleaning

The raw dataset contained metadata and Unicode-specific formatting that was not required for sentiment calculation.

* **Dimensionality Reduction:** Removed descriptive columns like `Unicode codepoint` and `Unicode block`.
* **Standardization:** Utilized Regular Expressions (Regex) to convert all column headers into `snake_case` for programmatic consistency.

### 2. Feature Engineering

To provide a more granular view of emotion, a custom sentiment variable was calculated:


* **Sentiment Score:** A continuous variable ranging from -1 to +1.
* **Positive Flag:** A Boolean classifier ( if ) to facilitate rapid querying and categorical analysis.

### 3. Exploratory Data Analysis (EDA)

Used `pandas` querying to segment emojis by usage frequency (Occurrences) and positioning within the string to see if "introductory" emojis differ from "concluding" emojis.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git

```


2. **Navigate to Project:**
`Data cleaning/emoji sentiment project/`
3. **Install Dependencies:**
Ensure you have `pandas` and `jupyter` installed:
```bash
pip install pandas jupyter

```


4. **Run the Notebook:**
Open `Emoji Sentiment.ipynb` and execute the cells to reproduce the analysis.

---

## 🖼 Visualizations

> **Note:** The following are placeholders for visualizations generated within the notebook.

* **:** A bar chart showing the ratio of positive vs. negative emojis.
* **:** A scatter plot illustrating where positive and negative emojis typically land in a sentence.

---

**Developed by:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
**Repo Location:** [Cisco Data Science Program](https://github.com/BhavikBuchke/Cisco-Data-science-program/tree/main/Data%20cleaning/emoji%20sentiment%20project)

Created as part of the **Cisco Data Science Program**.
