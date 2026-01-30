
---

# 🚗 Auto MPG Dataset — Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project explores the **Auto MPG dataset** from the UCI Machine Learning Repository, which contains specifications and fuel efficiency data for cars manufactured between **1970–1982**.

The goal is to:

* **Understand trends** in fuel efficiency across years, origins, and engine types
* **Uncover relationships** between MPG, engine displacement, horsepower, weight, and acceleration
* **Identify patterns** that explain how automotive engineering and market trends evolved during the dataset period

This notebook demonstrates **data cleaning**, **visual exploration**, and **insight generation** — essential skills for any data analyst or data scientist.

---

## 📂 Dataset Information

The dataset contains **398 entries** with the following attributes:

| Column       | Description                                |
| ------------ | ------------------------------------------ |
| mpg          | Miles per gallon (fuel efficiency)         |
| cylinders    | Number of engine cylinders                 |
| displacement | Engine displacement (cubic inches)         |
| horsepower   | Engine horsepower                          |
| weight       | Vehicle weight (lbs)                       |
| acceleration | Time to accelerate from 0–60 mph (seconds) |
| model year   | Year of manufacture                        |
| origin       | 1 = American, 2 = European, 3 = Japanese   |
| car name     | Model name of the car                      |

---

## 🛠️ Methodology

1. **Data Loading & Inspection**

   * Checked data types, null values, and initial structure
2. **Data Cleaning**

   * Replaced missing `horsepower` values (originally '?') with median values
   * Detected and treated outliers using the **IQR method**
3. **Exploratory Data Analysis**

   * Univariate analysis: Histograms, KDE plots for each numeric feature
   * Categorical analysis: Count plots for `cylinders`, `origin`, and `model year`
   * Bivariate analysis: Scatter plots and correlations to explore feature relationships
4. **Feature Scaling**

   * Applied MinMax scaling for normalized visualizations (only for comparison, not used in core insights)

---

## 📊 Key Insights

* **Fuel Efficiency Trends**:
  Fuel efficiency improved in later years, influenced by the 1973 oil crisis and changing regulations.
* **Engine Size vs MPG**:
  Cars with higher displacement and horsepower tend to have lower MPG.
* **Vehicle Origins**:

  * American cars dominate the dataset but tend to be less fuel-efficient
  * Japanese cars consistently show higher MPG
  * European cars occupy a middle ground
* **Acceleration**:
  Most vehicles have moderate acceleration times (14–16 seconds), reflecting balanced engineering priorities of the era.

---

## 🎨 Visualizations

Some of the key plots include:

* **MPG Distribution** — skewed right, indicating fewer highly fuel-efficient cars
* **Displacement Distribution** — smaller engines more common, but still relatively large by modern standards
* **Horsepower Distribution** — most cars between 70–110 HP, with a secondary performance peak
* **Origin Counts** — custom-colored (Red = USA, Blue = Europe, Yellow = Japan)
* **Correlation Heatmap** — shows strong negative correlation between weight and MPG

---

## 🚀 Next Steps

* Develop a **predictive regression model** for MPG
* Explore clustering to group vehicles by performance and efficiency
* Compare trends to modern datasets for historical context

---

## 💻 Tech Stack

* Python 3
* Pandas, NumPy
* Matplotlib, Seaborn
* Jupyter Notebook

---

## 📜 References

* [UCI Machine Learning Repository — Auto MPG Dataset](https://archive.ics.uci.edu/ml/datasets/auto+mpg)
* [Seaborn Documentation](https://seaborn.pydata.org/)

---

**Author:** *Srijan Sen*
📧 *[srijansen201@gmail.com](mailto:srijansen201@gmail.com)* | 🔗 [LinkedIn](https://www.linkedin.com/in/srijan-sen-b2505222a/) | 💻 [GitHub](https://github.com/web-dev-champ/)

---
