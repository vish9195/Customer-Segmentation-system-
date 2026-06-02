# Customer Segmentation System

> RFM-based customer segmentation for a bicycle and car sales company — 11 distinct customer groups identified from transaction history, visualised in a Tableau dashboard.

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat&logo=tableau&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

---

## Problem Statement

The company had no structured view of which customers drive revenue, which are at risk of churning, and which are low-value one-time buyers. Without this, marketing spend was spread uniformly across all customers regardless of potential return.

---

## Approach — RFM Analysis

RFM scores each customer on three dimensions:

| Dimension | Meaning |
|---|---|
| **Recency (R)** | How recently did they purchase? |
| **Frequency (F)** | How often do they purchase? |
| **Monetary (M)** | How much do they spend in total? |

Customers are scored 1–5 on each dimension, then grouped into **11 actionable segments**:

| Segment | Description |
|---|---|
| Champions | Bought recently, buy often, spend the most |
| Loyal Customers | Buy regularly with good spend |
| Potential Loyalists | Recent buyers with moderate frequency |
| New Customers | Bought very recently for the first time |
| Promising | Recent but low frequency |
| Need Attention | Above-average RFM but not recent |
| About to Sleep | Below-average recency, frequency, and spend |
| At Risk | Used to buy often but haven't recently |
| Can't Lose Them | Made large purchases but haven't returned |
| Hibernating | Low RFM across all dimensions |
| Lost | Lowest recency, frequency, and spend |

---

## Dataset

- `CustomerDemographic_Cleaned.csv` — customer profiles (age, gender, job, wealth segment)
- `Transactions_Cleaned.csv` — purchase transaction history

Both files are cleaned versions of the source data, included in the repo.

---

## Files

```
Customer-Segmentation-system/
├── Customer Segmentation.ipynb   # Full analysis notebook
├── CustomerDemographic_Cleaned.csv
├── Transactions_Cleaned.csv
└── README.md
```

---

## Key Outputs

- RFM scores for every customer
- 11 segment labels with customer counts
- Tableau dashboard visualising segment distribution, revenue by segment, and demographic overlays

---

## Setup & Usage

```bash
# Clone the repo
git clone https://github.com/vish9195/Customer-Segmentation-system-.git
cd "Customer-Segmentation-system-"

# Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# Launch Jupyter
jupyter notebook "Customer Segmentation.ipynb"
```

---

## Tech Stack

- **Python / Pandas** — RFM score calculation and data wrangling
- **Matplotlib / Seaborn** — in-notebook visualisations
- **Tableau** — interactive segment dashboard

---

## Author

**V P Vishal** — Master of Business Analytics, University of Auckland  
[GitHub](https://github.com/vish9195) · [Email](mailto:vishalvp1963@gmail.com)
