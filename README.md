# CloudTask Pro — SaaS Churn & Revenue Intelligence

## Project Overview

A Python business analytics project examining customer churn,
subscription revenue, churn drivers, and unit economics for a
B2B SaaS project management company.

**Reporting period:** January 2022 – December 2025.

## Business Questions

- Which subscription plans and customer segments have high churn?
- How do churn and monthly recurring revenue change over time?
- Why do customers cancel their subscriptions?
- How do historical customer revenue and acquisition cost compare?
- Which non-churned customers show potential retention risks?

## Datasets

- `subscriptions.csv`: 600 subscription records.
- `monthly_revenue.csv`: 48 months of revenue and customer metrics.

Both CSV files should be placed alongside the notebook.

## Key Findings

| Metric | Result |
|---|---|
| Customers analyzed | 600 |
| Historically churned customers | 313 |
| Historical customer churn proportion | 52.17% |
| Latest reported MRR | $292,628.61 |
| Latest reported monthly churn | 1.42% |
| Weighted CAC benchmark | $202.20 |
| At-risk non-churned customers | 23 |

### Churn Insights

**Highest-risk subscription plan:**
Starter at
70.51% observed churn.

**Billing-cycle comparison:**
Monthly billing: 60.51% observed churn.
Annual billing: 40.32% observed churn.

### Top Three Churn Reasons

- Budget Cuts: 53 customers
- Price Too High: 51 customers
- Company Closed: 48 customers

## Recommended Business Actions

1. Prioritize investigation of churn among Starter customers.
2. Evaluate onboarding, engagement, and renewal support for
   customers with low feature usage and low NPS.
3. Review pricing concerns and customer feedback before
   designing retention interventions.

## Technology

- Python
- pandas
- NumPy
- Matplotlib
- Google Colab / Jupyter Notebook

## How to Run

1. Download or clone this repository.
2. Place both CSV files in the same working directory
   as `CloudTask_Analysis.ipynb`.
3. Install dependencies:

```bash
python -m pip install -r requirements.txt
```

4. Open the notebook in Jupyter or Google Colab.
5. Execute the cells from top to bottom.

**Colab note:** Uploaded runtime files are temporary.
Upload the two CSVs again when starting a new Colab session.

## Methodology and Limitations

- The overall 52.17% is a historical customer churn
  proportion, not a monthly churn rate.
- Monthly churn percentages come from the revenue dataset.
- Observed churn proportions may reflect differing customer
  tenures and exposure periods.
- The historical CLV proxy uses completed lifespans of
  churned customers only and excludes ongoing customers.
- The CAC figure is an acquisition-weighted monthly
  benchmark, not verified plan-specific CAC.
- Revenue-to-CAC ratios are not profit margins.
- True Net Revenue Retention cannot be derived from the
  available aggregate MRR fields.
- Usage and NPS risk indicators are exploratory rules,
  not validated churn predictions.
- Segment associations do not establish causation.

## Portfolio Scope

This project demonstrates data exploration, customer
segmentation, revenue analysis, business metrics,
visualization, and evidence-based recommendations.
