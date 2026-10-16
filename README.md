# Healthcare Dataset Exploratory Data Analysis

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on a healthcare dataset to understand patient demographics, medical conditions, admission patterns, billing amounts, and insurance-related information.

The analysis uses Python libraries such as **Pandas, NumPy, Matplotlib, and Seaborn** to explore and visualize different aspects of the healthcare dataset.

## 📂 Dataset

The dataset used in this project is:

```text
healthcare_preprocessed (1).csv
```

The dataset contains **54,966 patient records** and **18 columns**.

### Dataset Columns

- `Name`
- `Age`
- `Gender`
- `Blood_Type`
- `Medical_Condition`
- `Admission_Date`
- `Doctor`
- `Hospital`
- `Insurance_Provider`
- `Billing_Amount`
- `Room Number`
- `Admission_Type`
- `Discharge_Date`
- `Medication`
- `Test_Results`
- `Length_of_Stay`
- `Age_Group`
- `Admission_Urgency`

The dataset contains:

- **14 categorical columns**
- **3 integer columns**
- **1 floating-point column**
- All 54,966 records have non-null values.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## 📦 Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

## 🔍 Exploratory Data Analysis

The project investigates several important characteristics of the healthcare dataset.

### 1. Dataset Overview

The notebook loads the CSV file and examines:

- Number of rows
- Number of columns
- Column names
- Data types
- Missing values
- Basic dataset structure

The dataset contains **54,966 rows and 18 columns**.

## 📊 Visualizations

### Patient Age Distribution

A histogram with KDE is used to understand the distribution of patient ages.

**Visualization:**
- Distribution of Patient Ages

### Patient Age Distribution by Gender

The age distribution is further analyzed based on gender using a histogram with gender as the grouping variable.

**Visualization:**
- Patient Age Distribution by Gender

### Gender Distribution

A bar chart is used to show the number of patients belonging to each gender category.

**Visualization:**
- Patient Distribution by Gender

### Medical Condition Distribution

The number of patients for each medical condition is analyzed.

The medical conditions included are:

- Arthritis
- Asthma
- Cancer
- Diabetes
- Hypertension
- Obesity

**Visualization:**
- Number of Patients by Medical Condition

### Gender Distribution by Medical Condition

A count plot is used to examine how gender is distributed across different medical conditions.

**Visualization:**
- Gender Distribution by Medical Condition

### Admission Type Distribution

The dataset contains three admission types:

- Elective
- Emergency
- Urgent

A bar chart is used to analyze the distribution of patients across these admission types.

### Medical Condition vs Admission Type

A cross-tabulation is created between medical condition and admission type.

| Medical Condition | Elective | Emergency | Urgent |
|---|---:|---:|---:|
| Arthritis | 3062 | 3073 | 3083 |
| Asthma | 3069 | 2978 | 3048 |
| Cancer | 3114 | 2988 | 3038 |
| Diabetes | 3031 | 2988 | 3197 |
| Hypertension | 3182 | 2975 | 2994 |
| Obesity | 3015 | 3100 | 3031 |

A stacked bar chart is also used to visualize admission types across medical conditions.

## 💰 Billing Analysis

### Billing Amount Distribution

A histogram with KDE is used to examine the distribution of patient billing amounts.

### Billing Amount by Medical Condition

A violin plot is used to compare billing amount distributions across different medical conditions.

The average billing amount for each medical condition is calculated.

| Medical Condition | Average Billing Amount |
|---|---:|
| Obesity | 25,804.36 |
| Diabetes | 25,660.48 |
| Asthma | 25,633.46 |
| Arthritis | 25,511.78 |
| Hypertension | 25,503.06 |
| Cancer | 25,152.32 |

Based on the calculated averages, **Obesity has the highest average billing amount**, while **Cancer has the lowest average billing amount** among the listed medical conditions.

### Billing Amount by Insurance Provider

A violin plot is used to analyze the distribution of billing amounts across different insurance providers.

This helps visualize how billing amounts vary between insurance providers.

## 📈 Key Analysis Areas

The notebook focuses on:

1. Patient age distribution
2. Patient distribution by gender
3. Medical condition distribution
4. Gender distribution across medical conditions
5. Admission type distribution
6. Relationship between medical conditions and admission types
7. Billing amount distribution
8. Billing amount across medical conditions
9. Average billing amount by medical condition
10. Billing amount distribution by insurance provider

## 📁 Project Structure

```text
Project/
│
├── Task6_EDA.ipynb
├── healthcare_preprocessed (1).csv
└── README.md
```

## ▶️ How to Run the Project

1. Download or clone the project.
2. Place `healthcare_preprocessed (1).csv` in the required location.
3. Open `Task6_EDA.ipynb` using Jupyter Notebook, JupyterLab, or Google Colab.
4. Make sure the required Python libraries are installed.
5. Run the notebook cells sequentially.
6. Review the generated tables and visualizations.

## 🎯 Objective

The main objective of this project is to explore the healthcare dataset and identify patterns in:

- Patient demographics
- Medical conditions
- Hospital admissions
- Admission types
- Billing amounts
- Insurance providers

## ✅ Conclusion

This exploratory data analysis provides an overview of the healthcare dataset and its major characteristics. Different statistical summaries and visualizations are used to understand patient demographics, medical conditions, admission patterns, and billing amounts.

The analysis shows that the dataset contains **54,966 patient records across 18 attributes**, providing information about patients, their medical conditions, hospital admissions, billing, medications, insurance providers, and length of stay.

The analysis also calculates average billing amounts by medical condition, with **Obesity having the highest average billing amount (25,804.36)** and **Cancer having the lowest (25,152.32)** among the conditions analyzed.
