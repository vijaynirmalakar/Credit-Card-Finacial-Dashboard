# Credit Card Financial Dashboard — Customer & Transaction Report
> Analyzed 10,108 credit card customers and 655,700+ transactions worth $55.3M in annual revenue using Power BI to uncover spending patterns, card performance, and customer segmentation insights for a financial services business.

---

## Problem
The credit card business had two separate data sources — customer demographics and transaction records — but no unified view of:
- Which card categories and customer segments generate the most revenue
- How customers prefer to transact (swipe vs chip vs online) and what they spend on
- Whether revenue is stable across quarters or concentrated in specific periods
- Which states, jobs, and education levels drive the highest transaction volumes

This project merges both data sources and builds a 2-page Power BI dashboard answering all these questions with quarterly drill-through and multi-filter capabilities.

---

## Dataset
| File | Description | Size |
|---|---|---|
| `credit_card.csv` | Card category, transactions, interest, fees, utilization, chip usage, expenditure type | 10,108 rows × 18 columns |
| `customer.csv` | Age, gender, income, job, education, marital status, state, satisfaction score | 10,108 rows × 15 columns |

- **Period:** 2023 (Q1–Q4)
- **Joined on:** Client_Num (one-to-one relationship)
- **Total combined columns after merge:** 32 attributes per customer

---

## Tools Used
`Power BI` `DAX` `Power Query` `Data Modelling` `Financial Analytics` `Customer Segmentation`

---

## Process

1. **Data Understanding** — Explored two CSVs: credit_card.csv (transaction-level) and customer.csv (demographic-level); identified Client_Num as the join key
2. **Data Modelling** — Merged both tables in Power BI via one-to-one relationship on Client_Num; verified no null or duplicate keys
3. **Data Cleaning** — Standardized card category labels, income group binning, age group segmentation in Power Query
4. **DAX Measures** — Created: Total Revenue (Trans + Interest + Fees), Total Interest Earned, Avg Credit Limit, Avg Utilization Ratio, Avg Customer Satisfaction Score, Delinquent Account Count
5. **Dashboard Page 1 (Customer Report)** — Revenue by job, age group, gender, salary group, education, marital status, top 5 states, dependent count — with Q1–Q4 and card type filters
6. **Dashboard Page 2 (Transaction Report)** — Revenue by card category, expenditure type, chip usage, education, quarterly trend chart, revenue by customer job — with same filter set
7. **Insights** — Derived 6 actionable business recommendations across card strategy, customer targeting, and risk management

---

## Dashboard Preview

### Page 1 — Customer Report
<img width="1264" height="707" alt="Credit Card Customer Report" src="https://github.com/user-attachments/assets/dc145389-da6a-4978-8121-678460b79041" />


### Page 2 — Transaction Report
<img width="1260" height="711" alt="Credit Card Transaction Report" src="https://github.com/user-attachments/assets/5d412fd4-d60d-46c6-b741-c6f950029a70" />


---

## Key Findings

- **Blue card dominates with 83.5% of total revenue** — generating $46.1M out of $55.3M total; Silver, Gold, and Platinum together contribute just 16.5%
- **Businessmen are the #1 customer segment** — $14.3M in transaction amount (32.1% of total), nearly 1.5× more than the next segment (White-collar at $8.2M)
- **Swipe transactions lead at $27.9M (62.7%)** vs Chip ($13.9M, 31.1%) and Online ($2.8M, 6.2%) — online adoption is critically low
- **Bills is the top expenditure category at $11.0M** followed by Entertainment ($7.6M) and Fuel ($7.5M) — essentials dominate spending
- **Q3 is the peak revenue quarter at $11.4M** — consistent quarterly performance overall (range: $10.7M–$11.4M), showing stable business
- **40–50 age group generates the highest revenue at $20.2M (45.5%)** — the core customer segment, nearly double the 30–40 group ($9.1M)
- **Graduates drive the most transactions at $18.0M** — more than double that of High School customers ($8.9M)
- **TX and NY are top states** at $10.3M and $10.3M respectively — nearly tied, with CA close at $10.1M
- **614 delinquent accounts identified** — 6.1% of the customer base posing active credit risk
- **Only 6.2% of revenue comes from online transactions** — a significant digital adoption gap in 2023
- **57.5% of customers activated their card within 30 days** — indicating strong initial engagement but room to improve

---

## Business Recommendations

1. **Diversify beyond Blue card** — 83.5% revenue concentration in one tier is a business risk; create upgrade incentives to push Silver/Gold adoption
2. **Launch online transaction campaigns** — only 6.2% of revenue is online; offer cashback or rewards for digital payments to grow this channel
3. **Target 40–50 age Businessmen in TX, NY, CA** — this specific profile combines the highest age-group revenue, top job segment, and top states
4. **Monitor 614 delinquent accounts proactively** — early intervention (payment reminders, restructuring offers) reduces write-off risk
5. **Build Graduate-focused card products** — graduates generate 40.3% of transaction revenue; a premium card with education benefits could increase loyalty
6. **Improve card activation beyond 30 days** — 42.5% of customers are slow activators; an onboarding nurture sequence could unlock latent revenue

---

## Project Structure
```
credit-card-financial-dashboard/
├── credit_card.csv              # Transaction & card data (10,108 rows, 18 cols)
├── customer.csv                 # Customer demographics (10,108 rows, 15 cols)
├── Credit_Card_Dashboard.pbix   # Power BI report file
├── dashboard_customer.png       # Customer report screenshot
├── dashboard_transaction.png    # Transaction report screenshot
└── README.md                    # This file
```

---

## Author
**Vijay Nirmalakar**
[[LinkedIn Profile](https://www.linkedin.com/in/vijaynirmalakar/)] | [[GitHub Profile](https://github.com/vijaynirmalakar)]

*Tools: Power BI | DAX | Power Query | Domain: Financial Analytics, Credit Risk, Customer Segmentation*
