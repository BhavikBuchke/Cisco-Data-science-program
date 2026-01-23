# 🐾 Any Animal Except... | Analyzing Linguistic Trends of British Menageries

---

## 📈 Executive Summary

During the expansion of the British Empire (1750–1835), exotic animals were brought to England and displayed in **menageries**—the precursors to modern zoos. This project utilizes data science to explore a historical-linguistic hypothesis: **Did the physical exhibition of animals directly influence the frequency of those animal names in the English language?**

By analyzing word-frequency datasets, we compare "popular" menagerie animals (like Tigers and Ostriches) against "difficult" animals that were rarely exhibited (like Hummingbirds and Meerkats) to identify clear cultural patterns in language usage.

---

## 🎯 Business & Research Problem

Historically, cultural shifts are often visible through language. The core problem this project addresses is **quantifying cultural impact**.

For a museum or historical researcher, understanding which events (like the opening of a menagerie) triggered spikes in public interest is vital. We aim to differentiate between general "exoticism" and the specific influence of **physical presence and accessibility** on public discourse.

---

## 🛠 Technical Workflow

### 1. Data Acquisition & Preparation

The analysis relies on two primary CSV datasets containing longitudinal word frequency data:

* `animal-word-trends.csv`: General animal mention frequencies.
* `animal-word-trends-menageries.csv`: Targeted data for specific exotic species.

### 2. Comparative Analysis

We categorized species into two distinct groups to test our explanatory mechanism:

* **Exhibited Group:** Animals successfully kept and displayed (e.g., Tiger, Ostrich).
* **Scarcity Group:** Animals that were too fragile or difficult to keep in 18th-century captivity (e.g., Hummingbird, Penguin).

### 3. Data Visualization

Using `Matplotlib`, we developed custom plotting functions to overlay the "Menagerie Period" (1750–1835) as a visual span. This allows for immediate visual correlation between the era of exhibition and the rise in literary mentions.

---

## 💡 Key Insights & Results

The data reveals a stark contrast between animals that the public could see in person versus those they only read about in scientific texts:

| Animal Category | Linguistic Trend | Conclusion |
| --- | --- | --- |
| **Exhibited Animals** (Tiger, Macaw) | **Sharp Increase** | Physical exhibition acted as a "viral" catalyst for language usage. |
| **Difficult Animals** (Hummingbird, Penguin) | **Flat/Stagnant** | Lack of physical presence resulted in significantly lower cultural penetration. |

**The Explanatory Mechanism:**
The physical accessibility of animals in menageries created a feedback loop: public viewing led to more frequent mentions in journals, newspapers, and literature, effectively "normalizing" the exotic creature within the common English lexicon.

---

## 🖼️ Visualizations

*(Below are examples of the trends generated in the notebook)*

### The "Exhibition" Effect
The chart below tracks animals frequently and successfully displayed in British menageries. Note the significant uptick in mentions (frequency per million words) that accelerates during the Menagerie Period (1750–1835), represented by the shaded region.

<img width="900" height="500" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/10f866d2-2212-4783-91ae-b329bd20da69" />

### The "Scarcity" Effect
In contrast, animals that were difficult to keep in captivity or only known through remote scientific reports show a much flatter trend. Despite their "exotic" nature, they did not permeate the cultural lexicon as deeply.

<img width="900" height="500" alt="Code_Generated_Image(1)" src="https://github.com/user-attachments/assets/d6aad14c-9b80-426c-b6ea-c73e51aa0894" />

---

## 🚀 How to Run

To explore these trends yourself, follow these steps:

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Story Telling/Any Animal Except Project"

```


2. **Install Dependencies:**
```bash
pip install pandas matplotlib

```


3. **Open the Notebook:**
Launch `animal word trends.ipynb` in Jupyter Notebook or VS Code.
4. **Upload Data:**
Ensure `animal-word-trends-menageries.csv` is in the same directory as the notebook.

---

### 🧰 Tech Stack

* **Language:** Python
* **Libraries:** Pandas (Data Wrangling), Matplotlib (Visualization)
* **Platform:** Jupyter Notebook / Google Colab

---

*Created as part of the **Cisco Data Science Program**.*
