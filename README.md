# 📊 Insurance Pricing Analytics — Simulated Data Project

This project showcases the potential of **data-driven pricing strategies** in the insurance sector using a **simulated national dataset**. The goal is to demonstrate how machine learning can be applied to detect pricing inefficiencies, simulate business impact, and guide strategic decisions.

> ⚠️ **Disclaimer:** All data used in this project is **artificially generated** and **does not represent any real company, customer, or policy**. The financial figures and predictions are purely illustrative and represent a simulated nationwide insurance system, not the reality of any specific company.
![cover](https://github.com/user-attachments/assets/8cfd461c-e163-41fe-a7b7-04d9101327f3)


---

## 🧠 Project Overview

### Objectives
- Predict total claim costs per client using neural networks.
- Recommend premiums with a fixed business margin.
- Detect **underpriced**, **fairly priced**, and **overpriced** policies.
- Prioritize strategic adjustments in high-impact regions or coverage types.
- Simulate potential **revenue uplift** under different policy adjustment strategies.

### Dataset
The dataset is fully simulated and includes:
- Demographic and policyholder data
- Policy coverage types and regions
- Actual premiums and predicted claim costs

---

## 📌 Key Stages

### ✅ Stage 1: Predictive Modeling
- Trained a regression model to estimate total paid claims.
- Achieved a test MAE of ~230,000 Gs.

### ✅ Stage 2: Suggested Premiums
- Calculated suggested premiums with a 25% margin.
- Labeled policies as *Underpriced*, *Fairly Priced*, or *Overpriced*.

### ✅ Stage 3: Business Impact Simulation
- Estimated financial impact of mispriced premiums.
- Simulated potential uplift in revenue if adjustments were applied.

### ✅ Stage 4: Strategic Pricing Simulation
- Focused on clients with the highest underpricing gaps.
- Calculated how much premiums could be increased **without hurting demand**, based on elasticity assumptions.
- Simulated three revenue scenarios:
  - **Status Quo** (Current Premiums)
  - **Full Adoption** (Apply all suggested premiums)
  - **Conservative Policy** (Apply increases only to severely underpriced clients)

---

## 💡 Final Insights

- The conservative policy alone could **boost total revenue by over 1.2 trillion Gs (~170 million USD)**.
- Regions like *Central* and *San Pedro* and *Premium coverage clients* concentrate most of the underpricing margin.
- A flexible pricing model based on predicted risk can unlock **hidden profit opportunities** while maintaining fairness.

---

## 🗂️ File Structure
insurance-pricing-analytics/
├── insurance_pricing_analysis.ipynb # Main notebook
├── simulated_insurance_data.csv # Input data
├── outputs/ # Graphs and visualizations
├── README.md # This file
└── .gitignore # Python + Jupyter ignores


---

## 🔧 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/YOUR_USERNAME/insurance-pricing-analytics.git
   cd insurance-pricing-analytics

pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
jupyter notebook insurance_pricing_analysis.ipynb


