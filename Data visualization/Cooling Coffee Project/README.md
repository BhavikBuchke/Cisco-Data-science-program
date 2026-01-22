# Project: Thermal Dynamics of Coffee Cooling

> **Analyzing the science behind the perfect cup of coffee.**

## 📊 Executive Summary

This project investigates the thermal retention capabilities of various beverage containers over a 55-minute duration. By analyzing the cooling rates of coffee in a **Ceramic Mug**, an **Insulated Mug**, and an **Insulated Mug with a Lid**, we quantify the impact of container material and evaporative cooling on beverage temperature.

The results highlight a significant performance gap between open containers and sealed insulated systems, providing data-driven evidence for the effectiveness of modern travel mug designs.

---

## 🎯 The Business Problem

For the beverage industry and consumer goods manufacturers, "Time-to-Cold" is a critical metric for customer satisfaction.

* **The Conflict:** Ceramic mugs provide a traditional tactile experience but lose heat rapidly. Insulated mugs reduce conductive heat loss through walls but remain vulnerable to heat loss through the surface.
* **The Goal:** To determine which design element—insulation or the lid—contributes most significantly to heat retention, helping users make informed choices for their morning commute.

---

## 💡 Key Insights & Results

The data reveals that the presence of a lid is the single most influential factor in maintaining beverage heat, even more so than the insulation material itself.

| Container Type | Start Temp (°F) | End Temp (55 min) | Total Heat Loss |
| --- | --- | --- | --- |
| **Insulated with Lid** | 146.6 | **115.7** | **-30.9°F** |
| **Insulated (Open)** | 135.5 | 79.7 | -55.8°F |
| **Ceramic (Open)** | 128.8 | 76.6 | -52.2°F |

* **The "Lid Effect":** The insulated mug with a lid retained **~36°F more heat** than the same mug without a lid, proving that evaporative cooling and convection through the top are the primary drivers of cooling.
* **Insulation vs. Ceramic:** Interestingly, once the lid is removed, a standard insulated mug performs similarly to a ceramic mug, with both approaching room temperature (67°F) rapidly.
* **Drinkable Window:** Assuming the "ideal" drinking temperature is above 110°F, only the **Insulated with Lid** option kept the coffee within the preferred range for the entire hour.

---

## 🛠 Technical Workflow

### 1. Data Collection & Inspection

The dataset `hot-coffee.csv` contains time-series temperature recordings at 5-minute intervals. The data was loaded using `pandas` for initial exploratory analysis.

### 2. Visualization Engineering

To create a "Recruiter-Ready" chart, the following enhancements were made via `matplotlib`:

* **Direct Labeling:** Implemented a custom `add_end_labels` function to place category names directly at the end of data lines, eliminating the need for a distracting legend.
* **Minimalist Design:** Applied a "clean" style by removing unnecessary spines (top, right, and left) and utilizing a light grid to improve readability without clutter.
* **Baseline Context:** Added a horizontal dashed line at **67°F** to represent the ambient room temperature, providing a clear reference point for the cooling limit.

---

## 📈 Visualizations

### Coffee Cooling Rates by Container Type

The plot below illustrates the cooling trajectory of each container. The dramatic separation of the "Insulated with Lid" line showcases the superior thermal efficiency of sealed systems.

---

## 🚀 How to Run

To explore the analysis and generate the visualizations locally:

1. **Clone the repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data visualization/Cooling Coffee Project"

```


2. **Install dependencies:**
```bash
pip install pandas matplotlib

```


3. **Launch the Notebook:**
```bash
jupyter notebook "cooling coffee.ipynb"

```



---

## 📂 Project Structure

* `cooling coffee.ipynb`: The primary analysis file featuring Python code and visualization logic.
* `hot-coffee.csv`: Time-series temperature data for three container configurations.
* `coffee_cooling_analysis.png`: The finalized visualization for presentation.

---

**Created as part of the Cisco Data Science Program.**
