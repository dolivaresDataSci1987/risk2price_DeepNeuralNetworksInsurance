# 📊 Insurance Pricing Analytics — Simulated Data Project

This project showcases the potential of **data-driven pricing strategies** in the insurance sector using a **simulated national dataset**. The goal is to demonstrate how machine learning can be applied to detect pricing inefficiencies, simulate business impact, and guide strategic decisions.

![cover](https://github.com/user-attachments/assets/8cfd461c-e163-41fe-a7b7-04d9101327f3)

> ⚠️ **Disclaimer:** All data used in this project is **artificially generated** and **does not represent any real company, customer, or policy**. The financial figures and predictions are purely illustrative and represent a simulated nationwide insurance system, not the reality of any specific company.

---

## 🧠 Project Overview

### Objectives

- Predict total claim costs per client using a deep neural network (DNN).
- Recommend risk-adjusted premiums with a fixed business margin.
- Detect **underpriced**, **fairly priced**, and **overpriced** policies.
- Prioritize strategic adjustments by region and coverage type.
- Simulate potential **revenue uplift** under different premium adjustment strategies.

### Dataset

The dataset is fully simulated and includes:
- Demographic and policyholder features
- Coverage types and geographic region
- Actual premiums and claim histories

---

## 📌 Key Stages

### ✅ Stage 1: Predictive Modeling
- Trained a fully connected DNN to estimate `TotalPaidClaims` per client.
- Achieved a test MAE of approximately **230,000 Gs**, which corresponds to ~21% of the average claim cost (≈ 1.1 million Gs).

### ✅ Stage 2: Suggested Premiums
- Recommended premiums were calculated using:  
  `SuggestedPremium = PredictedClaimCost × 1.25`  
  (a 25% business margin).
- Policies were labeled based on the difference between actual and suggested premium.

### ✅ Stage 3: Business Impact Simulation
- Simulated the financial effect of correcting mispriced policies.
- Identified regions and coverage types with the largest hidden revenue gaps.

### ✅ Stage 4: Strategic Pricing Simulation
- Focused on severely underpriced clients only.
- Modeled three policy scenarios to estimate annual uplift:
  - **Status Quo** (no changes)
  - **Full Adoption** (apply all suggested premiums)
  - **Conservative Policy** (adjust only the most underpriced)

---

## 💡 Final Insights

- The conservative pricing policy yields a potential uplift of approximately **2.3 billion Gs (~330,000 USD)**.
- Regions such as *Central* and *San Pedro*, as well as *Premium coverage* clients, concentrate most of the underpricing margin.
- A flexible, model-driven pricing strategy enables more **granular and fair premium adjustments**, improving both profitability and market sustainability.

---

## 🚧 Future Improvements

- Add quantile-based loss functions to better capture extreme claim values.
- Include confidence intervals or uncertainty estimates for premium recommendations.
- Modularize the codebase into reusable scripts and functions for production.
- Benchmark against traditional actuarial methods (e.g., GLM, credibility theory).
- Integrate real-world elasticity data to validate behavioral assumptions.
