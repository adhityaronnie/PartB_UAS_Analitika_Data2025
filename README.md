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
A 1–2 page actuarial interpretation memo answering the interpretation questions (below)
