<div align="center">

<!-- Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=FFB800&height=200&section=header&text=Maximising%20Revenue%20for%20Drivers&fontSize=36&fontColor=ffffff&fontAlignY=38&desc=Data-Driven%20Insights%20for%20NYC%20Taxi%20Operations&descAlignY=58&descSize=16" width="100%"/>

<br/>

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![SciPy](https://img.shields.io/badge/SciPy-Statistics-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)](https://scipy.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C?style=for-the-badge&logo=python&logoColor=white)](https://matplotlib.org/)
[![Statsmodels](https://img.shields.io/badge/Statsmodels-Modeling-FF6F00?style=for-the-badge&logo=python&logoColor=white)](https://www.statsmodels.org/)

<br/>

> **Smarter insights. Better decisions. Higher earnings.**

<br/>

![Records](https://img.shields.io/badge/📊%20Dataset-6.4M%2B%20Records-FFB800?style=flat-square)
![Status](https://img.shields.io/badge/Status-Completed-28a745?style=flat-square)
![Domain](https://img.shields.io/badge/Domain-Transportation%20%7C%20FinTech-blue?style=flat-square)

</div>

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Research Questions](#-research-questions)
- [Dataset](#-dataset)
- [Methodology](#-methodology)
- [Key Findings](#-key-findings)
- [Hypothesis Testing](#-hypothesis-testing)
- [Recommendations](#-recommendations)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)

---

## 🚖 Overview

The taxi booking industry relies on **data-driven decisions** to maximise driver earnings and improve operational efficiency. This project analyses the relationship between **payment methods** and **fare amounts** using a dataset of **6.4+ million NYC taxi trip records** to identify patterns that influence revenue.

The insights help answer whether payment type affects fare pricing and support strategies for **maximising driver revenue** without compromising customer satisfaction.

---

## ❓ Research Questions

```
1. To what extent does the payment method impact the total fare collected?

2. Can strategic payment preferences be promoted to enhance driver revenue
   without affecting customer satisfaction?
```

---

## 📂 Dataset

**Source:** NYC Taxi Trip Dataset (6.4+ million records)

The dataset was cleaned and feature-engineered, retaining the following columns:

| Column | Description |
|--------|-------------|
| `passenger_count` | Number of passengers (1–5) |
| `payment_type` | Card or Cash |
| `fare_amount` | Total fare in USD |
| `trip_distance` | Distance in miles |
| `duration` | Trip duration in minutes *(derived feature)* |

> 🔧 `duration` was engineered as: `tpep_dropoff_datetime − tpep_pickup_datetime`

---

## 🔬 Methodology

```mermaid
flowchart LR
    A[🗃️ Raw Data\n6.4M+ Records] --> B[🧹 Data Cleaning\n& Feature Engineering]
    B --> C[📊 Descriptive\nAnalysis]
    C --> D[🧪 Hypothesis\nTesting]
    D --> E[💡 Insights &\nRecommendations]
```

| Step | Technique | Description |
|------|-----------|-------------|
| **1** | 🧹 Data Cleaning | Removed nulls, filtered outliers, retained relevant columns |
| **2** | 📊 Descriptive Analysis | Explored fare amounts, trip durations, and payment distributions |
| **3** | 🧪 Hypothesis Testing | Independent two-sample T-test on payment type vs. fare amount |
| **4** | 📈 Visualization | Distribution plots, pie charts, and passenger count breakdowns |

---

## 📊 Key Findings

### 💳 Payment Type Preference

<div align="center">

| Payment Method | Share of Transactions |
|:--------------:|:---------------------:|
| 💳 Card | **67.5%** |
| 💵 Cash | **32.5%** |

</div>

> Card payments dominate customer transactions, reflecting a strong customer preference for **digital, cashless experiences**.

---

### 🚕 Journey Insights

- 💳 **Card users** show a **higher average fare amount and trip distance** than cash users
- Customers are more likely to choose card payments for **longer, higher-value trips**
- Digital payment users represent **greater revenue potential** for drivers

---

### 👤 Passenger Count Breakdown

| Payment Type | 1 Passenger | 2 Passengers | 3+ Passengers |
|:------------:|:-----------:|:------------:|:-------------:|
| 💳 Card | 40.08% | 14% | ~13% |
| 💵 Cash | 20.04% | 7% | ~5% |

> **Solo travellers** are the dominant customer segment across all payment types.
> Trip frequency decreases as group size increases — larger groups prefer alternative transport.

---

## 🧪 Hypothesis Testing

```
H₀ (Null Hypothesis):     There is NO significant difference in average fare
                          between card and cash payments.

H₁ (Alternate Hypothesis): There IS a significant difference in average fare
                            between card and cash payments.
```

### Results

<div align="center">

| Metric | Value |
|:------:|:-----:|
| **Test Used** | Independent Two-Sample T-Test |
| **T-Statistic** | `169.21` |
| **P-Value** | `< 0.05` |
| **Decision** | ✅ Reject H₀ |

</div>

> **Conclusion:** There is a **statistically significant difference** in average fares between card and cash payments. Payment type is a meaningful factor in **customer spending behaviour** and should be central to revenue optimisation strategies.

---

## 💡 Recommendations

```
┌─────────────────────────────────────────────────────────────────┐
│  💳  Encourage Card Payments                                     │
│      Card transactions → higher fares + longer trips            │
│      = greater revenue for drivers                               │
├─────────────────────────────────────────────────────────────────┤
│  🎁  Introduce Digital Payment Incentives                        │
│      Cashback, discounts, or loyalty rewards                     │
│      to nudge customers toward card payments                     │
├─────────────────────────────────────────────────────────────────┤
│  ⚡  Enhance Digital Payment Experience                          │
│      Fast, secure, seamless card payment options                 │
│      to boost satisfaction and revenue simultaneously            │
└─────────────────────────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

<div align="center">

| Tool | Purpose |
|------|---------|
| ![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white&style=flat-square) | Core programming language |
| ![Pandas](https://img.shields.io/badge/-Pandas-150458?logo=pandas&logoColor=white&style=flat-square) | Data manipulation & analysis |
| ![Matplotlib](https://img.shields.io/badge/-Matplotlib-11557C?logo=python&logoColor=white&style=flat-square) | Data visualization & plotting |
| ![SciPy](https://img.shields.io/badge/-SciPy-8CAAE6?logo=scipy&logoColor=white&style=flat-square) | Statistical tests & distributions |
| ![Statsmodels](https://img.shields.io/badge/-Statsmodels-FF6F00?logo=python&logoColor=white&style=flat-square) | Statistical modelling & inference |

</div>

---

## 📁 Project Structure

```
📦 maximising-revenue-for-drivers
├── 📂 data/
│   └── nyc_taxi_trips.csv          # Raw dataset (6.4M+ records)
├── 📂 notebooks/
│   └── analysis.ipynb              # Full EDA + Hypothesis Testing
├── 📂 outputs/
│   ├── fare_distribution.png       # Fare distribution by payment type
│   ├── trip_distance_dist.png      # Trip distance distribution
│   └── payment_preference.png     # Pie chart of payment type share
├── 📂 reports/
│   └── Maximising_Revenue.pdf      # Final project report
├── requirements.txt
└── README.md
```

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=FFB800&height=100&section=footer" width="100%"/>

*Built with ❤️ using Python & NYC Open Data*

</div>
