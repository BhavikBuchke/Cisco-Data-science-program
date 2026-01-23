# 🐾 Plotting Animal Words | Data Storytelling with Historical Lexicon

---

## 📈 Executive Summary

How do historical breakthroughs like the invention of the automobile or the completion of a railway system change the way we write? This project explores **Data Storytelling** by analyzing the usage frequency of animal names in printed books over a 300-year span (1700–2019). By correlating linguistic shifts with real-world events, we uncover the hidden impact of technology, culture, and economy on our written records.

---

## 🎯 Business & Research Problem

Raw data alone is insufficient; context is what provides value. The challenge of this project is to move beyond simple plotting and into **hypothesis testing**. We address the following core questions:

* Can a linguistic trend serve as a proxy for social or technological shifts?
* How do we use explanatory mechanisms to separate coincidence from causation?
* Which animal "brands" (e.g., Cat vs. Dog) have historically dominated human interest?

---

## 💡 Key Insights & Results

The data reveals fascinating correlations between human progress and animal mentions:

| Hypothesis Case | Key Finding | Explanatory Mechanism |
| --- | --- | --- |
| **Horse & Automobile** | **Sharp Decline post-1886** | The invention of the "horseless carriage" reduced the horse's central role in daily life and literature. |
| **Lobster & Railway** | **Spike post-1869** | The transcontinental railway allowed fresh seafood to be transported inland, increasing its cultural and culinary popularity. |
| **Cats vs. Dogs** | **Dog Dominance** | "Dog" is mentioned nearly **2x more frequently** than "Cat" in the most recent historical records (2019). |
| **Cow & 1830** | **Unprecedented Peak** | Correlated with the Texas ranching boom and the formalization of veterinary science. |

### Visualizing the "Horse" Decline

Following the invention of the automobile in 1886, we see a distinct tapering of the word "horse" in literature, marking a major societal transition.

<img width="800" height="350" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/77a1e9ac-5110-4377-b3d8-5107c2c7ddb0" />

### The Pop Culture Shift: Penguins vs. Dinosaurs

This visualization compares the cultural footprint of two very different "celebrity" animals. While the "Penguin" saw early interest from polar expeditions, the "Dinosaur" captures the public imagination in a exponential trend starting in the mid-1900s.

<img width="800" height="350" alt="Code_Generated_Image(1)" src="https://github.com/user-attachments/assets/09915021-2007-4511-a70b-93e4964723c6" />

### The Popularity Contest: Cat vs. Dog

While both animals have seen a rise in mentions in the modern era, the "Dog" consistently leads in literary frequency.

<img width="800" height="450" alt="Code_Generated_Image(2)" src="https://github.com/user-attachments/assets/a86b2292-1b59-45f5-84ba-fb33ee78f75b" />

### Visualizing the 1830 Cattle Milestone
The year 1830 marked a turning point for cattle in the public record, coinciding with the end of cattle grazing on the Boston Common and the foundation of Texas ranching traditions. Note the linguistic peak aligned with the orange milestone marker.

<img width="800" height="350" alt="Code_Generated_Image(3)" src="https://github.com/user-attachments/assets/e8862596-49c2-4012-920d-9cc0c5be90eb" />

---

## 🛠 Technical Workflow

### 1. Data Processing

* **Normalization:** Frequency is measured as "occurences per million words published" to account for the increasing volume of books published annually.
* **Dataset:** Analyzed `animal-word-trends-intro.csv` containing longitudinal data for hundreds of species.

### 2. Tool Development

Created a modular, reusable Python function `plot_word_trend()` to:

* Extract specific animal subsets via Pandas `query()`.
* Generate standardized time-series visualizations.
* Overlay historical "markers" (vertical lines) to test correlation.

### 3. Hypothesis Testing

Evaluated specific timestamps—such as the 1830 cattle ranching shifts or the 1869 railway completion—to find evidence of "Explanatory Mechanisms" that explain why a word frequency spiked or crashed.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Story Telling/Plotting Animal Words Project"

```


2. **Install Dependencies:**
```bash
pip install pandas matplotlib

```


3. **Launch the Notebook:**
Open `plotting animal words.ipynb` in Jupyter or VS Code to explore the trends and test your own animal hypotheses.

---

### 🧰 Tech Stack

* **Language:** Python
* **Analysis:** Pandas (Querying & Filtering)
* **Visualization:** Matplotlib (Time-Series, Multi-trend overlay)
* **Concepts:** Data Storytelling, Hypothesis Testing, Explanatory Mechanisms

---

*Created as part of the **Cisco Data Science Program**.*
