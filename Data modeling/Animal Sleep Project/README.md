# Animal Sleep Analysis with Custom Linear Regression

## Project Overview

This project demonstrates my end-to-end data science workflow, combining data exploration, statistical modeling, and object-oriented Python design. Using an animal sleep dataset, I build and evaluate a custom linear regression model to analyze relationships between biological variables and sleep patterns.

**The repository highlights my ability to:**
1. Work with real-world datasets
2. Implement machine learning models from scratch using industry libraries
3. Structure reusable, maintainable Python code
4. Evaluate and visualize model performance
```
📂 Project Structure
├── animal-sleep.csv        # Dataset used for analysis
├── analysis.ipynb          # Jupyter Notebook with EDA, modeling, and visualization
├── linear_model.py         # Custom Linear Regression class
└── README.md               # Project documentation
```
## Dataset

**animal-sleep.csv** contains biological and behavioral attributes of animals, including sleep duration and related metrics.
The dataset is used to explore correlations and fit a linear regression model to predict outcomes based on selected features.

## Model Implementation

The project includes a reusable LinearModel class implemented in **linear_model.py**, which wraps **scikit-learn** functionality in a clean, object-oriented interface.

### Key Capabilities

1. Model fitting using **LinearRegression**
2. Automatic calculation of:
- Slope
- Intercept
- R² score
3. Visualization of regression lines


## Analysis Workflow (Notebook)

The Jupyter Notebook walks through:
**1. Data Loading & Cleaning**
- Importing CSV data with Pandas
- Handling missing or inconsistent values
**2.Visual exploration using Matplotlib**
**3.Model Training**
- Fitting the custom linear model
- Interpreting coefficients and goodness of fit
**4.Visualization**
- Plotting regression lines
- Comparing predicted vs. actual values

## Installation & Setup
**Prerequisites**

Python 3.8+
pip or conda

**Install Dependencies**
 ```
 pip install pandas matplotlib scikit-learn
```
## Usage
**Run the Notebook**
```
jupyter notebook analysis.ipynb
```

**Use the Model Programmatically**
```
from linear_model import LinearModel
model = LinearModel(model_name="Sleep Predictor")
model.fit(x, y)
model.print_model_info()
```

## Technologies Used

**Python**
**Pandas** – data manipulation
**Matplotlib** – visualization
**Scikit-learn** – regression and metrics
**Jupyter Notebook** – exploratory analysis

## Skills Demonstrated
Data analysis & visualization
Machine learning fundamentals
Object-oriented Python
Reproducible research practices
Clean, professional documentation

## Author

Bhavik Buchke
