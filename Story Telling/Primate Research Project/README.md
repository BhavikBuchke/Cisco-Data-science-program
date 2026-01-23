You are correct—the previous version only highlighted two of the three charts. I have updated the README below to ensure the **"Comparison of Other Animals"** chart has its own dedicated section and explanation, alongside the linguistic and usage trends.

---

# 🐒 Primate Research | Analyzing the "Animal Liberation" Impact

---

## 📈 Executive Summary

Can a single book change a culture? This project evaluates the impact of Peter Singer’s 1975 book, *Animal Liberation*, often credited with sparking the modern animal rights movement. By comparing **linguistic data** (how often we talk about animals) with **actual research data** (how many animals are used in labs), we uncover a complex narrative: while the movement successfully reduced the use of "pet-like" animals, it triggered a "Primate Paradox" where scientific necessity outweighs ethical discourse.

---

## 🎯 Business & Research Problem

Measuring the effectiveness of a cultural campaign requires looking at both sentiment and operations. This project treats the 1975 publication as a **variable of change** to determine:

1. **Linguistic Impact:** Did the book create a "shock" to the cultural system visible in written records?
2. **Success in Substitution:** Did the movement successfully reduce the research footprint for common laboratory species?
3. **The Primate Exception:** Why do primates remain the only animal group with a long-term increase in usage?

---

## 💡 Key Insights & Results

The data reveals that 1975 was a definitive "flashpoint" year that permanently altered the trajectory of animal research in the West.

| Metric | Observation | Outcome |
| --- | --- | --- |
| **Linguistic Peak** | **1975–1976** | Every primate-related term peaked immediately following the book's release. |
| **Other Animals** | **Sharp Decline** | Usage of dogs, cats, and rabbits has dropped significantly since the 1970s. |
| **Primate Usage** | **Growth of 456/year** | Primates are the only group with a long-term *increase* in research usage. |

---

## 📊 Visual Evidence

### 1. The Linguistic Flashpoint

The word usage data shows a massive cultural shift starting exactly in 1975. The publication of *Animal Liberation* brought primate research into the mainstream spotlight, leading to a surge in debate and publication that peaked almost instantly.

<img width="700" height="350" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/a554f354-a9f4-4503-838c-e1da84489d18" />

### 2. The Success of the Movement (Non-Primates)

The animal rights movement was highly effective at reducing the research footprint for many species. Since 1975, the number of dogs, cats, and rabbits used in research has seen a consistent and dramatic decline.

<img width="700" height="350" alt="Code_Generated_Image(1)" src="https://github.com/user-attachments/assets/3d47f9c0-5473-4f90-a65f-6cc28817018d" />

### 3. The Primate Paradox

Despite the cultural shift and ethical pressure, primate research has intensified. While other animal groups saw a decrease, primates likely became irreplaceable for complex biomedical research (e.g., neuroscience and vaccines), leading to a divergence between public sentiment and scientific practice.

<img width="700" height="350" alt="Code_Generated_Image(2)" src="https://github.com/user-attachments/assets/ca702652-31d6-4a80-abed-b6a780877a63" />


---

## 🛠 Technical Workflow

### 1. Data Integration

Combined two distinct datasets to create a multi-dimensional view:

* `animal-word-trends-primate-research.csv`: Linguistic frequency data from the Google Books corpus.
* `number-of-research-animals-per-year.csv`: Historical counts of animals used in laboratory research.

### 2. Time-Series Correlation

Plotted linguistic trends against operational research counts with a vertical marker for the 1975 publication date. This highlights where public discourse (the "Why") aligns—or fails to align—with industry practice (the "What").

### 3. Species-Level Comparative Analysis

Analyzed the "Substitution Hypothesis" by comparing primate trends against other common laboratory animals to quantify the effectiveness of ethical movements across different animal categories.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Story Telling/Primate Research Project"

```


2. **Install Dependencies:**
```bash
pip install pandas matplotlib

```


3. **Execute the Notebook:**
Launch `primate research.ipynb` in Jupyter or Google Colab.

---

### 🧰 Tech Stack

* **Language:** Python
* **Data Wrangling:** Pandas
* **Visualization:** Matplotlib
* **Focus:** Data Storytelling, Cultural Analytics

---

*Created as part of the **Cisco Data Science Program**.*
