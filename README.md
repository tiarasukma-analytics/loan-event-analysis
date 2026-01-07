# Investor Investment Process Analysis

This project analyzes the investment behavior of investors on a peer-to-peer lending platform using event-based transaction data.

The original project and dataset are provided by **DQLab** in Bahasa Indonesia and implemented in **R**.  
This repository contains my **Python translation and analysis**, focusing on investment flow and retention patterns.

---

## Business Context

DQLab Finance is a peer-to-peer lending platform where:
- Borrowers submit loan requests
- Loans are listed on a marketplace
- Registered investors browse, order, and fund loans

Understanding how investors move from registration to repeated investments is critical for improving retention and platform growth.

---

## Objectives

1. Analyze the end-to-end investment process
2. Measure time from registration to first investment
3. Build cohort-based retention analysis based on first investment month

---

## Dataset

- Source: DQLab Finance (educational dataset)
- Format: Event-level logs
- Key events:
  - `investor_register`
  - `investor_view_loan`
  - `investor_order_loan`
  - `investor_pay_loan`
  - `loan_to_marketplace`

---

## Methodology

### 1. Event Funnel Exploration
- Count unique investors and loans per event
- Analyze ordering and payment duration

### 2. Time to First Investment
- Identify first investment date per investor
- Measure conversion lag from registration

### 3. Cohort Retention Analysis
- Define cohorts based on first investment month
- Calculate months since first investment
- Measure investor retention by cohort

Retention is calculated as:

retention_rate = active_investors / cohort_size


---

## Key Output

- Cohort retention table showing investor activity by month since first investment
- Identification of early drop-off patterns after initial investment

---

## Tools Used

- Python
- pandas
- numpy

---

## Notes

- This project prioritizes analytical clarity over production-level optimization
- Some exploratory steps were intentionally retained to reflect real-world analysis workflows
