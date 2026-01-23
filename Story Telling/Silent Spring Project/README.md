# 🦅 Silent Spring | Pesticides, Population Collapses, & Cultural Awakening

---

## 📈 Executive Summary

In 1944, the introduction of DDT was hailed as a "miracle" for pest control. However, by 1962, Rachel Carson’s *Silent Spring* warned of a looming ecological catastrophe. This project uses **data storytelling** to analyze how these two major milestones altered the course of history. By cross-referencing linguistic trends of 300 years with biological datasets, we quantify the transition from a society focused on "conquering" nature to one focused on "conserving" it.

---

## 🎯 Business & Research Problem

How do we prove that a single book or a single chemical changed the collective consciousness? For environmental historians and data scientists, the challenge is linking **macro-trends in literature** (word frequency) to **micro-biological data** (eggshell thinning).

This project addresses the following questions:

1. **Direct Correlation:** Did the usage of "pest" words drop as DDT gained popularity?
2. **Biological Validation:** Is there physical evidence in the data (e.g., eggshell thickness) that supports the claims made in *Silent Spring*?
3. **The "Carson Effect":** Can we see the birth of the modern environmental movement in the recovery of bird-related mentions post-1962?

---

## 💡 Key Insights & Results

The analysis reveals a stark divergence between how humans discuss "pests" vs. "protected species."

| Species Group | Linguistic Trend | Drivers |
| --- | --- | --- |
| **Insects** (Fly, Louse, Bedbug) | **Continuous Decline** | The "success" of synthetic pesticides reduced insects from a public preoccupation to a background nuisance. |
| **Birds of Prey** (Peregrine, Osprey) | **U-Shaped Trend** | A collapse in mentions post-1944 (population crash) followed by a **massive surge** post-1962 (awareness/recovery). |
| **Sparrowhawks** | **Sharp Biological Drop** | Eggshell thickness plummeted **immediately** after DDT's public release in 1944. |

---

## 📊 Visual Evidence

### 1. The Decline of the Pest

Following the 1944 release of DDT, the frequency of insect-related words in literature continued a steep decline, reflecting a world that believed it had finally "won" the war against pests.

<img width="800" height="350" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/c391da5c-354e-440c-95d7-d78cf265d865" />

### 2. Biological Proof: Eggshell Thinning

The data confirms Rachel Carson’s warning: almost immediately after DDT introduction (1944), the physical health of bird populations (measured by eggshell thickness) entered a catastrophic decline.

<img width="800" height="300" alt="Code_Generated_Image(2)" src="https://github.com/user-attachments/assets/818228f7-c341-45da-9f9d-08d3b5469e24" />

### 3. The "Silent Spring" Recovery

The publication of *Silent Spring* in 1962 acted as a cultural catalyst. Mentions of vulnerable birds like the Robin and Peregrine Falcon skyrocketed as they became symbols of the nascent environmental movement.

<img width="800" height="350" alt="Code_Generated_Image(1)" src="https://github.com/user-attachments/assets/312d1948-064e-4606-b142-2055fa3a212a" />


---

## 🛠 Technical Workflow

### 1. Multi-Source Data Analysis

We analyzed two complementary datasets:

* `animal-word-trends-silent-spring.csv`: Longitudinal linguistic data (1900–2014).
* `sparrowhawk-eggshell-data.csv`: Biological metrics tracking population health across the 20th century.

### 2. Comparative Analysis

We categorized species into **"Pests"** (Insects) and **"Apex Predators/Songbirds"** (Birds) to observe the different ways technology and literature interact with the food web.

### 3. Historical Correlation

Using Python's `Matplotlib`, we overlaid vertical markers for **1944 (DDT availability)** and **1962 (Silent Spring)**. This allows for a "Time-Series Intervention" analysis, identifying the exact moment cultural sentiment shifted.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Story Telling/Silent Spring Project"

```


2. **Install Dependencies:**
```bash
pip install pandas matplotlib

```


3. **Open the Notebook:**
Launch `silent spring.ipynb` in Jupyter Notebook or VS Code to view the full analysis.

---

### 🧰 Tech Stack

* **Language:** Python
* **Libraries:** Pandas (Data Wrangling), Matplotlib (Time-Series Visualization)
* **Concepts:** Data Storytelling, Biomagnification Analysis, Environmental History

---

*Created as part of the **Cisco Data Science Program**.*
