# Car Dimensions: A Decade-by-Decade Evolution Analysis

> **Analyzing the intersection of automotive design and urban constraints.**
## 📊 Executive Summary

In the automotive world, "size inflation" is a well-documented phenomenon. Modern cars are often significantly larger than their predecessors of the same model name. This project quantifies this trend by analyzing 53 iconic car models, comparing the physical dimensions of their **First Generation** to their **Latest Generation**.

By calculating growth in length, width, and height, this study highlights how cars have expanded to accommodate safety features, technology, and consumer demand, and what that means for our urban environments.

---

## 🎯 The Business Problem

Urban infrastructure—such as parking garage spaces, residential driveways, and narrow city lanes—was largely standardized decades ago.

* **The Conflict:** As car "footprints" (Length × Width) increase, compatibility with existing infrastructure decreases.
* **The Goal:** To provide a data-driven look at which car segments (compacts vs. SUVs) are growing the fastest and to visualize the trajectory of automotive scaling.

---

## 💡 Key Insights & Results

The analysis shows a near-universal increase in size across all 53 models.

| Metric | Observation |
| --- | --- |
| **Length Growth** | Every single model in the dataset grew in length, with some increasing by over **20%**. |
| **Width Expansion** | Width showed the most consistent upward trend, often to meet modern side-impact safety standards. |
| **Footprint Bloat** | Small hatchbacks from the 1970s have frequently grown to match the dimensions of 1990s-era luxury sedans. |

* **Growth Leader:** Models like the **Suzuki Jimny** and **Mini Cooper** (noted in similar datasets) show dramatic scaling to meet modern safety and comfort requirements.
* **Infrastructure Impact:** The average "footprint" increase suggests that a modern "compact" car often occupies as much road space as a previous generation's "mid-size" car.

---

## 🛠 Technical Workflow

### 1. Data Cleaning & Segmentation

Using `pandas`, the `car-dimensions.csv` dataset was split into two distinct groups: `first_generation` and `latest_generation`. We used the `brand_model` as the primary key to merge these datasets into a single comparison frame.

### 2. Feature Engineering

Beyond raw dimensions, we engineered several new metrics:

* **Absolute Change:**  in mm for length, width, and height.
* **Percentage Change:** Normalized growth rates to compare small cars vs. large trucks fairly.
* **Car Footprint:** Calculated as `Length * Width` to represent the total ground area occupied by the vehicle.

### 3. Data Visualization

Visualized the "Size Inflation" using:

* **Paired Scatter Plots:** To show the distribution of growth relative to an identity line ().
* **Sorted Bar Charts:** Identifying the "Top Growers" in the automotive industry.

---

## 📈 Visualizations

### 1. Length & Width Scaling

The following scatter plots compare the original generation (X-axis) against the modern version (Y-axis). Points above the red dashed line indicate models that have grown.

<img width="500" height="300" alt="Code_Generated_Image(3)" src="https://github.com/user-attachments/assets/1e157315-4909-4ca9-87b9-37c37b0f7354" />
<img width="500" height="300" alt="Code_Generated_Image(4)" src="https://github.com/user-attachments/assets/4aea66ce-91fb-4b97-8766-2019caf2a175" />


### 2. Top Growth Trends

This chart highlights the 10 car models with the most significant percentage increase in length.

<img width="500" height="300" alt="Code_Generated_Image(5)" src="https://github.com/user-attachments/assets/e673af9e-57e2-4429-9b79-d3eda824699f" />


---

## 🚀 How to Run

To replicate this analysis and explore the data:

1. **Clone the repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data visualization/Car Dimensions Project"

```


2. **Install requirements:**
```bash
pip install pandas matplotlib

```


3. **Run the Notebook:**
```bash
jupyter notebook "Car dimensions.ipynb"

```



---

## 📂 Project Structure

* `Car dimensions.ipynb`: The Jupyter notebook containing the full Python analysis.
* `car-dimensions.csv`: Dataset covering 53 car models with first/latest generation specs.
* `car_length_analysis.png`: Scatter plot visualization for length.
* `car_width_analysis.png`: Scatter plot visualization for width.
* `car_growth_trends.png`: Ranking of models by growth percentage.

---

**Created as part of the Cisco Data Science Program.**
