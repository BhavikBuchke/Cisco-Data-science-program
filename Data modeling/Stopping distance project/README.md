# Physics of Safety: Analyzing E-Bike and Car Stopping Distances

## 📋 Executive Summary

This project explores the critical relationship between speed and safety in urban transportation. By analyzing stopping distance data for both E-bikes and cars, this study utilizes linear and polynomial modeling to determine how braking requirements escalate as velocity increases. The findings emphasize that stopping distance does not grow linearly with speed; rather, it follows a quadratic pattern, highlighting significant safety risks at higher velocities for both cyclists and drivers.

## ❓ The Problem

As E-bikes become a staple of urban commuting, understanding their mechanical limitations is essential for infrastructure planning and rider safety. A common misconception is that doubling your speed only doubles your stopping distance.

This project seeks to:

1. **Model the Physics:** Determine if the relationship between speed and stopping distance is linear or quadratic.
2. **Cross-Vehicle Comparison:** Compare the braking efficiency of E-bikes versus standard automobiles.
3. **Speed Categorization:** Analyze how braking behavior changes between "low-speed" and "high-speed" E-bike operation.

---

## 🛠️ Technical Workflow

The analysis followed a data-driven approach grounded in physical principles:

1. **Data Ingestion & Wrangling:**
* Processed multiple datasets: `car-stopping-distances.csv`, `ebike-stopping-distances.csv`, and granular high/low-speed E-bike data.


2. **Feature Engineering:**
* Converted raw speed and distance metrics into usable formats for regression analysis.


3. **Comparative Modeling:**
* Applied **Linear Regression** to test basic correlations.
* Evaluated **Quadratic/Polynomial** fits to account for the kinetic energy formula (), where stopping distance is proportional to the square of the velocity.


4. **Visual Analytics:**
* Created scatter plots with regression overlays to visualize the "braking curve" for different vehicle types.



---

## 📈 Key Insights & Results

The data confirms that as speed increases, the distance required to stop grows at an accelerating rate.

| Vehicle Type | Observations |
| --- | --- |
| **E-Bikes** | Exhibit a clear non-linear increase in stopping distance as they move from low to high speeds. |
| **Cars** | While having more braking power, they require significantly more space due to higher mass and momentum. |
| **Safety Threshold** | The "Total Stopping Distance" is heavily influenced by speed, making reaction time even more critical at higher velocities. |

**Core Findings:**

* **The Power of Speed:** Stopping distance follows a quadratic relationship. Doubling the speed roughly **quadruples** the stopping distance, a vital insight for road safety policy.
* **Mass Matters:** Even at similar speeds, the mass difference between a car and an E-bike results in vastly different kinetic energy levels, requiring distinct safety margins.
* **E-Bike Variability:** High-speed E-bike data suggests that mechanical braking systems must be specifically tuned for the higher velocities these vehicles can reach compared to traditional bicycles.

---

## 💻 How to Run

To replicate this study:

1. **Clone the Repository:**
```bash
git clone https://github.com/BhavikBuchke/Cisco-Data-science-program.git
cd "Data modeling/Stopping distance project"

```


2. **Install Requirements:**
```bash
pip install pandas matplotlib numpy scikit-learn

```


3. **Execute the Analysis:**
Open `E-bikes stopping distance.ipynb` in your preferred Jupyter environment. Ensure all `.csv` data files are in the same directory as the notebook.

---

## 🎓 Program Credits

Created as part of the **Cisco Data Science Program**. This project demonstrates the application of regression analysis to physical safety and urban transit engineering.

---

**Author:** [Bhavik Buchke](https://www.google.com/search?q=https://github.com/BhavikBuchke)
