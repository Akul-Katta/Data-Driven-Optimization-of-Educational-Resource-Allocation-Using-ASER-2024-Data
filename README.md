# 📊 Data-Driven Optimization of Educational Resource Allocation Using ASER 2024 Data

## Overview

This project was developed for **NSS Open Projects 2026 – Analytics & Insights Track (Challenge 5.3)**.

The objective is to identify educational factors most strongly associated with student learning outcomes and develop an evidence-based framework for educational resource allocation.

Using state-level data from the **Annual Status of Education Report (ASER) 2024**, the project evaluates how digital access, school infrastructure, and educational standards relate to Grade VIII reading performance across Indian states.

---

## Problem Statement

Educational programs often involve multiple interventions such as infrastructure development, teacher deployment, and digital learning initiatives. However, resource allocation decisions are frequently made without clear evidence regarding which interventions contribute most to student outcomes.

This project aims to:

* Identify factors associated with reading performance.
* Quantify the relative importance of different interventions.
* Propose a data-driven budget allocation strategy.
* Support evidence-based educational planning.

---

## Dataset

### Source

**ASER 2024 (Annual Status of Education Report)**

### Coverage

* 22 Indian States
* 30 Educational Indicators
* State-level aggregated data

### Categories

| Category              | Variables                                                        |
| --------------------- | ---------------------------------------------------------------- |
| Learning Outcomes     | Grade VIII Reading Ability                                       |
| Digital Access        | Smartphone Access, Smartphone Usage, Online Educational Activity |
| School Infrastructure | Playground, Drinking Water, Toilets, Girls' Toilets              |
| Educational Standards | PTR Compliance, CTR Compliance                                   |

---

## Methodology

The project follows a six-stage analytical pipeline:

```text
ASER Dataset
      ↓
Data Cleaning
      ↓
Correlation Analysis
      ↓
OLS Regression
      ↓
Random Forest Analysis
      ↓
Budget Allocation Model
```

### Analytical Techniques

* Pearson Correlation Analysis
* Ordinary Least Squares (OLS) Regression
* Random Forest Feature Importance
* Data Visualization
* Budget Allocation Modeling

---

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Statsmodels
* Scikit-Learn
* Jupyter Notebook

---

## Key Findings

### Correlation with Grade VIII Reading Performance

| Variable                | Correlation Coefficient |
| ----------------------- | ----------------------- |
| Smartphone Access       | 0.37                    |
| Smartphone Usage        | 0.35                    |
| Playground Availability | 0.33                    |
| PTR Compliance          | 0.24                    |

### Random Forest Feature Importance

| Factor                  | Importance (%) |
| ----------------------- | -------------- |
| Smartphone Usage        | 40.09          |
| Smartphone Access       | 28.85          |
| Playground Availability | 19.43          |
| PTR Compliance          | 11.63          |

### Main Insight

Digital-access indicators account for nearly **69% of total feature importance**, suggesting that digital inclusion is strongly associated with improved reading outcomes.

---

## Budget Allocation Framework

Based on the analysis, the recommended resource allocation strategy is:

| Investment Area            | Allocation (%) |
| -------------------------- | -------------- |
| Smartphone Usage Programs  | 40.09          |
| Smartphone Accessibility   | 28.85          |
| Playground Development     | 19.43          |
| PTR Compliance Improvement | 11.63          |

### Priority Order

1. Digital Learning Programs
2. Smartphone Accessibility
3. School Infrastructure
4. Teacher Availability

---

## Results

### Top Performing States

| State            | Reading Score (%) |
| ---------------- | ----------------- |
| Mizoram          | 90.7              |
| Himachal Pradesh | 88.3              |
| Kerala           | 84.5              |
| Haryana          | 82.7              |
| Punjab           | 82.2              |

### Lowest Performing States

| State           | Reading Score (%) |
| --------------- | ----------------- |
| Andhra Pradesh  | 56.2              |
| Jammu & Kashmir | 58.5              |
| Karnataka       | 62.1              |
| Tamil Nadu      | 64.2              |
| Assam           | 65.9              |

---

## Project Structure

```text
NSS_Project/
│
├── data/
│   └── ASER_Master_Dataset_2024.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── images/
│   ├── correlation_heatmap.png
│   ├── state_ranking.png
│   ├── feature_importance.png
│   └── budget_allocation.png
│
├── report/
│   └── Project_Report.pdf
│
├── presentation/
│   └── Project_Presentation.pptx
│
├── requirements.txt
│
└── README.md
```

---

## Limitations

* Observational state-level dataset.
* Correlation does not imply causation.
* Small sample size (22 states).
* Single-year cross-sectional analysis.
* Actual outcome improvements require field implementation and longitudinal evaluation.

---

## Future Work

* District-level educational analysis.
* Multi-year ASER trend analysis.
* Integration with UDISE+ datasets.
* Causal impact evaluation using longitudinal data.
* Advanced predictive modeling for policy planning.

---

## Conclusion

This project demonstrates how statistical analysis and machine learning can support evidence-based educational planning. The results suggest that digital learning access and smartphone-enabled educational engagement exhibit the strongest associations with student reading outcomes, providing actionable insights for policymakers and educational stakeholders.

---

### Developed For

**NSS Open Projects 2026**
**Challenge 5.3 – Data-Driven Optimization of a Social Program**
**Track: Analytics & Insights**
