# 📊 Telco Customer Churn — Business Analytics Case Study

**AnalystLab Africa Data Analytics Internship — Week 5, Batch B**

A business analytics case study answering: *why are customers leaving the company, and which factors contribute most to churn?* Built on the [Telco Customer Churn dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) (7,043 customers, 21 variables).

---

## 🎯 Business Problem

The company is losing a significant share of customers to churn. Retention resources are limited, so this analysis identifies **which customer segments and behaviors drive churn**, to help the business prioritize where retention spend will have the greatest impact.

## 🔑 Key Findings

| Driver | Finding |
|---|---|
| **Contract type** | Churn drops from **42.7%** (month-to-month) → 11.3% (one year) → **2.8%** (two year) |
| **Internet service** | Fiber optic customers churn at **41.9%** vs. 19.0% for DSL |
| **Payment method** | Electronic check payers churn at **45.3%**, ~3x the rate of autopay customers |
| **Tenure** | Churned customers average **18 months** tenure vs. 38 months for retained customers |
| **Add-on services** | Customers without online security or tech support churn **2.5–3x** more |
| **Demographics** | Senior citizens (41.7%), and customers without a partner (33.0%) or dependents (31.3%), churn more |

**Overall churn rate: 26.54%** (1,869 of 7,043 customers)

<p align="center">
  <img src="outputs/charts/01_Churn_Distribution.png" width="320" alt="Overall churn distribution pie chart">
</p>

<p align="center">
  <img src="outputs/charts/08_Contract_Churn_Rate.png" width="400" alt="Churn rate by contract type">
  <img src="outputs/charts/09_Internet_Churn_Rate.png" width="400" alt="Churn rate by internet service">
</p>

## 💡 Recommendations

1. Incentivize longer contracts, prioritizing month-to-month customers in their first 12 months
2. Investigate the fiber optic experience — pricing, reliability, competitive positioning
3. Migrate electronic check payers toward automatic payment methods
4. Bundle and proactively promote online security and tech support add-ons
5. Build an early-tenure retention program focused on a customer's first year
6. Tailor retention outreach for senior citizens and single customers without dependents

## 🛠️ Tools & Skills

Python (pandas, numpy, matplotlib, seaborn) · exploratory data analysis · data cleaning · correlation analysis · segment/cross-tab analysis · business insight generation · stakeholder reporting

## 📁 Repository Structure

```
telco-churn-analysis/
├── scripts/
│   └── churn_analysis.py       # full analysis: cleaning, EDA, charts, tables
├── reports/
│   ├── Telco_Churn_Case_Study_Report.docx
│   └── Telco_Churn_Case_Study_Deck.pptx
├── outputs/
│   ├── charts/                 # 27 saved PNG visualizations (generated on run)
│   └── tables/                 # saved CSV tables (generated on run)
├── data/                       # place WA_Fn-UseC_-Telco-Customer-Churn.csv here (not tracked)
├── requirements.txt
└── README.md
```

## ▶️ How to Run

1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) and place `WA_Fn-UseC_-Telco-Customer-Churn.csv` in a `data/` folder.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the analysis:
   ```bash
   python scripts/churn_analysis.py
   ```
4. Charts save to `outputs/charts/`, tables save to `outputs/tables/`.

> Originally developed in Google Colab; the script above uses relative paths so it also runs locally.

## 📄 Deliverables

- **[Business Analytics Case Study Report](reports/Telco_Churn_Case_Study_Report.docx)** — full write-up with findings, insights, and recommendations
- **[Presentation Deck](reports/Telco_Churn_Case_Study_Deck.pptx)** — 8-slide stakeholder summary

---

*Part of the AnalystLab Africa Data Analytics Internship Program.*
`#BusinessAnalytics` `#DataAnalytics` `#DataScience` `#AnalystLabAfrica`
