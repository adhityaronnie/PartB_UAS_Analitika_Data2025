You are given a synthetic portfolio of life insurance policies observed over time. Some policies have an observed claim event (death/TPD/CI), 
while others are right-censored (admin censoring or lapse). Policies also have delayed entry (left truncation) via entry_month.
Files survival_policies.csv (main survival dataset; includes censoring + delayed entry)
survival_claims.csv (only event rows; claim amount and cause)
Allowed packages
Use Python 3.10+ with: pandas, numpy, matplotlib, scipy, lifelines
Install if needed:
pip install lifelines scipy pandas matplotlib numpy
What you must submit (deliverables)
A clean notebook/script that:
Loads data, validates it, and documents assumptions
Produces required tables/figures
Fits models and evaluates them on train/test split
A 1–2 page actuarial interpretation memo answering the interpretation questions (please look on the instruction pdf)

Dataset 1: survival_policies.csv (n=2500)
- policy_id: unique policy identifier
- entry_month: delayed entry time (months since study start). Use for left truncation.
- duration_months: observed follow-up time since entry (months). This is the survival duration.
- event: 1 = claim/death event observed, 0 = right-censored (admin censoring or lapse)
- age_at_entry: age at entry (years)
- gender: F/M
- smoker: 0/1
- product_type: TERM10, TERM20, WHOLE
- region_risk: Low, Med, High
- sum_assured_k: sum assured (in thousands of currency units)
- annual_premium_k: annual premium (in thousands)
- split: train/test indicator for model validation

Dataset 2: survival_claims.csv (only event=1 rows)
- policy_id: links to policies
- duration_months: time to claim since entry
- cause: Death/TPD/CI
- claim_amount_k: amount paid (in thousands)
- notification_lag_days: reporting lag
- claim_month: calendar month since study start when claim occurs
