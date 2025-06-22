# 📦 First Order Discount A/B Test — Food Delivery Platform

## Project Overview

This project evaluates the impact of first-order discounts on new customer GMV (Gross Merchandise Value) for an online food delivery platform.  
A simulated A/B test assigned new users to four discount groups: **0%**, **10%**, **20%**, and **30%**.  

The goal is to determine whether offering larger discounts leads to greater revenue on first orders — helping the business optimize discount strategy while balancing profitability.

---

## Business Motivation

Discounts are commonly used to acquire new users — but excessive discounts reduce margin and may not increase customer spend.  

This analysis identifies the optimal first-order discount level to maximize GMV and minimize unnecessary promotional costs.

---

## Data

- 21,321 total orders  
- 11,607 first orders  
- **11,497 delivered first orders** included in the analysis (non-delivered orders excluded)

---

## Methods

- Simulated A/B test with four balanced groups (0%, 10%, 20%, 30%)  
- Exploratory Data Analysis (EDA)  
- Independent t-tests for statistical significance  
- GMV uplift % calculation vs 0% control  
- Visualizations: boxplots, barplots with error bars

---

## Key Results

| Discount Group | GMV Uplift vs 0% | p-value (vs 0%) |
|----------------|------------------|-----------------|
| 0%             | 0.00 %           | —               |
| 10%            | +2.67 %          | 0.1765          |
| 20%            | -0.57 %          | 0.7541          |
| 30%            | -2.27 %          | 0.1982          |

- The **10% discount** produced a small positive GMV uplift, but was not statistically significant.  
- **20%** and **30%** discounts reduced GMV compared to the 0% control.  
- Only **10% vs 30%** showed a significant difference (p = 0.0081), favoring the 10% discount.

---

## Final Recommendation

✅ A **10% first-order discount** is optimal — providing moderate uplift without margin loss.  
❌ Higher discounts (20%, 30%) do not improve GMV and may reduce profitability.  

**Recommendation:** Implement a 10% discount for first orders. Avoid larger discounts.

