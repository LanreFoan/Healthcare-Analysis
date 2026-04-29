# 🏥 Healthcare Dataset — Exploratory Data Analysis

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-EDA-green?logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-orange)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## 📌 Project Overview

This project performs an end-to-end **Exploratory Data Analysis (EDA)** on a synthetic healthcare dataset sourced from [Kaggle](https://www.kaggle.com/). The dataset contains **55,500 patient records** spanning demographics, medical conditions, billing, admissions, and test results.

The goal is to surface meaningful trends and patterns that could inform healthcare decision-making — such as which conditions are most prevalent, how billing varies by admission type, and what factors associate with abnormal test results.

---

## 📂 Repository Structure

```
healthcare-eda/
│
├── healthcare_dataset-analysis.ipynb   # Main EDA notebook
├── healthcare_dataset.csv              # Raw dataset (from Kaggle)
├── README.md                           # Project documentation
└── assets/                             # Saved visualizations
    ├── AgeDis.png
    ├── BldTypFreq.png
    ├── AdmissionTrend.png
    ├── TimeseriesTrend.png
    └── BillingVariation.png
```

---

## 📊 Dataset Description

| Feature | Description |
|---|---|
| `Age` | Patient age |
| `Gender` | Male / Female |
| `Blood Type` | Patient blood type |
| `Medical Condition` | Diagnosed condition (e.g. Cancer, Diabetes) |
| `Date of Admission` | Hospital admission date |
| `Insurance Provider` | Patient's insurer |
| `Billing Amount` | Total billed amount (USD) |
| `Admission Type` | Emergency / Elective / Urgent |
| `Discharge Date` | Date of discharge |
| `Medication` | Medication prescribed |
| `Test Results` | Normal / Abnormal / Inconclusive |

> **Source:** [Kaggle — Healthcare Dataset](https://www.kaggle.com/)  
> **Records:** 55,500 rows · 15 columns

---

## 🔍 Analysis Sections

1. **Data Cleaning & Preprocessing** — null checks, duplicate removal, date parsing, feature engineering (`Stay Duration`)
2. **Univariate Analysis** — age distribution, condition frequency, medication usage
3. **Bivariate Analysis** — blood type by gender, conditions by gender, admission trends over time
4. **Billing Analysis** — billing variation across admission types and stay duration
5. **Test Results Analysis** — abnormal result patterns by condition and stay length
6. **Statistical Testing** — Chi-Square tests for independence between categorical variables

---

## 💡 Key Findings

- **Medical conditions** (Cancer, Diabetes, Obesity, Hypertension, Arthritis, Asthma) are evenly distributed across the dataset.
- **Billing Amount** varies widely across all admission types — patient-specific factors drive cost more than urgency of admission.
- **Stay Duration** is slightly longer for patients with Abnormal test results.
- A **Chi-Square test** revealed that Gender is significantly associated with Admission Type (p < 0.05), while Medical Condition and Test Results show no statistically significant dependence.
- **Admission trends** remain stable across years with no major seasonal spikes.

---

## 🛠️ Tools & Libraries

| Tool | Purpose |
|---|---|
| `pandas` | Data manipulation & aggregation |
| `numpy` | Numerical operations |
| `matplotlib` | Base plotting |
| `seaborn` | Statistical visualizations |
| `plotly` | Interactive charts |
| `scipy` | Chi-Square statistical testing |

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/healthcare-eda.git
cd healthcare-eda
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn plotly scipy
```

### 3. Run the notebook
```bash
jupyter notebook healthcare_dataset-analysis.ipynb
```

> ⚠️ Make sure `healthcare_dataset.csv` is in the same directory as the notebook before running.

---

## 👤 Author

**Your Name**  
Data Science Intern Candidate  
[LinkedIn](https://linkedin.com/in/yourprofile) · [GitHub](https://github.com/YOUR_USERNAME)

---

## 📄 License

This project is open-source under the [MIT License](LICENSE).
