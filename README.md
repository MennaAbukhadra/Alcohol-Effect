# Alcohol Effect on Student Performance (Machine Learning Project)

## Overview
This project analyzes how **alcohol consumption and lifestyle factors** influence students' academic performance.

A **Machine Learning classification model** was built to predict whether a student will **pass or fail** based on several features such as study time, family relationships, absences, free time, and weekend alcohol consumption.

---

## Dataset
- **549 student records**
- **15 features**

### Key Features
- sex
- age
- address
- parent status (Pstatus)
- father job (Fjob)
- studytime
- activities
- internet access
- romantic relationship
- family relationship (famrel)
- free time (freetime)
- weekend alcohol consumption (**Walc**)
- health
- absences
- final grade (**G3**)

---

## Target Variable
The final grade **G3** was converted into a classification variable:

- **1 → Pass (G3 ≥ 10)**
- **0 → Fail (G3 < 10)**

New column created: **G3_class**

---

## Data Preprocessing
Main preprocessing steps:

- Handling missing values
  - Numerical features → **median**
  - Categorical features → **mode**

- Converting categorical variables using **One-Hot Encoding**
- Creating the target column **G3_class**
- Splitting the dataset:
  - **80% Training**
  - **20% Testing**

---

## Exploratory Data Analysis
EDA was used to understand relationships between variables.

Visualizations include:
- Pass vs Fail distribution
- Correlation heatmap
- Feature importance visualization

---

## Machine Learning Model
Model used:

**Random Forest Classifier**

### Model Parameters
- `n_estimators = 100`
- `random_state = 6`

---

## Model Performance
**Accuracy: 0.89**

The model correctly predicts student performance in **89% of cases**.

---

## Important Features
Most influential factors affecting student performance:

- Study time
- Absences
- Weekend alcohol consumption
- Free time
- Family relationship quality

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
