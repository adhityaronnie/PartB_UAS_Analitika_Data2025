Assignment 4 (Week 9): Unsupervised Learning for Policyholder Segmentation
Course: Data Analytics for Actuarial Science
Week: 9
Topics: PCA, K-Means, Hierarchical Clustering
Dataset: policyholder_churn.csv (or similar policyholder dataset)
Deliverables:
1 Jupyter Notebook (Assignment4_unsupervised.ipynb)
2–3 page report (PDF) summarizing findings and actuarial interpretation
Weight: ~15% (adjust as you like)
Background (for students)
Insurance companies often group policyholders into segments for pricing, marketing, and retention strategies.
In this assignment, you will use unsupervised learning (PCA + clustering) to discover natural groups in a portfolio of policyholders.
Assume you have the dataset policyholder_churn.csv with variables:
age – policyholder age
tenure_years – years with the insurer
num_claims – number of claims filed
policy_type – Life / Health / Motor
annual_premium – annual premium charged
churn – 1 if the policyholder lapsed, 0 otherwise
For this assignment, use only the explanatory variables (age, tenure_years, num_claims, policy_type, annual_premium) for PCA and clustering. You may use churn later only for interpretation, not for training.
