# Day 16: Customer Lifetime Value (CLV) Estimate

## Objective
Introduce practical CLV estimation by utilizing historical purchase behavior to project future customer value and segment the customer base accordingly.

## Technical Implementation
Transitioned to advanced business logic using Python and Pandas to analyze a sample of the 'Online Retail II' dataset. 

1. **Base Metric Calculation:** Aggregated raw transactional data to calculate Total Revenue, Purchase Frequency (Order Count), and Average Order Value (AOV) per unique Customer ID.
2. **Method Comparison:**
   * **Historical CLV:** Calculated the absolute sum of all past purchases to determine current realized value.
   * **Predictive CLV:** Projected future value using a multiplier method.
3. **Stating Assumptions:** For the Predictive CLV model, a standard customer retention lifespan of 3 years was assumed based on historical retail baselines.
4. **Segment Analysis:** Deployed the `pd.qcut()` function to automatically distribute and classify the customer base into 'Low Value', 'Medium Value', and 'High Value' tiers based on their Predictive CLV output.

## Deliverables
Generated a complete CLV Table mapping individual customer IDs to their Historical CLV, Predictive CLV, and final Value Segment.
