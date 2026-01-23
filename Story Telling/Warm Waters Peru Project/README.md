# 🌊 Warm Waters off Peru | El Niño and the Anchoveta Fishery Crisis

---

## 📈 Executive Summary

Centuries ago, Peruvian fishing communities identified a recurring climate pattern they called "El Niño." This project uses data science to investigate the profound relationship between these ocean warming events and the **Peruvian Anchoveta**—historically one of the world's most productive fisheries.

By analyzing 50+ years of catch data alongside linguistic trends, we uncover a fascinating **"Inverse Correlation"**: while El Niño events decimated physical fish populations, they triggered massive spikes in global discourse and scientific documentation, marking a permanent shift in how humanity manages ecological crises.

---

## 🎯 Business & Research Problem

Ecological disasters don't just affect the ocean floor; they impact global economies and the historical record. The core problem this project addresses is **quantifying the cultural and economic response to a collapse**.

Specifically, we investigate the **Great Anchoveta Crash of 1972**. For a fishery that accounted for a significant portion of global fishmeal production, a collapse wasn't just a biological event—it was a global economic shock. This project identifies how these shocks leave a "linguistic footprint" that serves as an early indicator of social and scientific concern.

---

## 💡 Key Insights & Results

The analysis identifies a clear divergence between the **"Physical Catch"** and the **"Linguistic Catch"** during environmental extremes.

| Event | Physical Impact | Linguistic Impact | Insight |
| --- | --- | --- | --- |
| **Pre-1972 Growth** | **Exponential** | **Gradual Rise** | Anchoveta became a global economic powerhouse. |
| **1972 El Niño** | **Catastrophic Drop** | **Sharp Spike** | The collapse shifted "anchoveta" from a commercial term to a topic of crisis management. |
| **Species Shift** | **Replacement** | **Divergence** | As Anchoveta crashed, mentions of alternate species (Sardine, Mackerel) increased as the industry pivoted. |

---

## 📊 Visual Evidence

### 1. The Great Collapse (1972)

The physical catch of Anchoveta peaked at nearly **17 megatonnes** in 1970 before plummeting to almost zero following the 1972 El Niño. This represents one of the largest fishery collapses in history.

<img width="800" height="400" alt="Code_Generated_Image" src="https://github.com/user-attachments/assets/bb185402-2664-4672-b5cd-b5309c093306" />

### 2. The Linguistic Crisis Response

While the fish disappeared from the nets, they appeared more frequently in books and journals. The spike in word frequency during the crash highlights that "Anchoveta" transitioned from an industry commodity to a global case study for ecological fragility.

<img width="800" height="400" alt="Code_Generated_Image(1)" src="https://github.com/user-attachments/assets/fd918f7e-4193-452f-8ac3-77551d2ffa14" />

### 3. Shift in Cultural Focus

As the primary fishery collapsed, the public and scientific record began to track alternative species like **Sardines** and **Mackerel** more closely, reflecting an industry-wide pivot in search of stability.

<img width="800" height="400" alt="Code_Generated_Image(2)" src="https://github.com/user-attachments/assets/6f78eed8-3b82-4960-8271-8b4224a37e13" />

---

## 🛠 Technical Workflow

### 1. Multi-Dimensional Data Merging

We integrated economic production data (`anchoveta-caught-per-year.csv`) with cultural frequency data (`animal-word-trends-peru.csv`) to observe the lag between environmental changes and societal awareness.

### 2. Time-Series Analysis

Focused on the 1960–1980 window to capture the rise and fall of the Peruvian "economic miracle." We utilized `Matplotlib` to visualize the relationship between catch volume (in Megatonnes) and linguistic frequency (per million words).

### 3. Hypothesis Testing: The "Crisis Spike"

We tested the hypothesis that ecological disasters increase linguistic frequency. By comparing Anchoveta (which crashed) to Hake and Bonito (which remained stable), we confirmed that the "Linguistic Spike" is a unique indicator of ecological volatility.

---

## 🚀 How to Run

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Story Telling/Warm Waters Peru Project"

```


2. **Install Dependencies:**
```bash
pip install pandas matplotlib

```


3. **Execute the Notebook:**
Launch `warm waters peru.ipynb` in your preferred Jupyter environment. Ensure both CSV datasets are in the same folder.

---

### 🧰 Tech Stack

* **Language:** Python
* **Analysis:** Pandas (Merging & Aggregation)
* **Visualization:** Matplotlib
* **Concepts:** El Niño/Southern Oscillation (ENSO) Impact, Ecological Economics

---

*Created as part of the **Cisco Data Science Program**.*
