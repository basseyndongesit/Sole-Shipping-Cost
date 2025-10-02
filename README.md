# Sole Shipping: Optimizing Pre-Launch Shipping Strategy Through Data Simulation & A/B Testing

## Executive Summary

Sole Capsule, a pre-launch sneaker preservation startup, faced a critical business decision: how to structure its shipping pricing to maximize customer acquisition and profitability. Without historical sales data, I built a comprehensive shipping cost simulation in Excel, analyzed global shipping patterns, and conducted a data-driven A/B test simulation in Python to evaluate a "Free Shipping" strategy. The analysis revealed that offering "Free Shipping" at a higher product price could increase conversion rates by 35.7% and profitability, provided it achieves modest conversion lifts. I recommended implementing this strategy with close performance monitoring.

## Business Problem

As a pre-launch company, Sole Capsule had no customer data to answer fundamental go-to-market questions:
- What is the most cost-effective way to ship products globally?
- Which shipping carriers offer the best rates for key markets?
- How should we price shipping to maximize conversions and profit?
- Would a "Free Shipping" strategy be profitable despite higher upfront costs?

Core Challenge: Making data-driven shipping decisions in a complete data vacuum before the first customer order.

## Methodology

To solve this zero-data problem, I implemented a three-phase analytical approach:
#### Phase 1: Cost Infrastructure Development
1. Created a simulated shipping cost engine in Excel with 300+ synthetic orders.
2. Structured data across multiple interconnected sheets:
- Variable Assumptions: Product dimensions, weight, shipping origins.
- Carrier Zones: Geographic mapping to carrier-specific zones.
- Rates Table: Actual carrier pricing for standard/express shipping.
- MainData: Complete order simulation with realistic shipping costs.
- Dashboard: Pivot tables for initial cost analysis.

#### Phase 2: Exploratory Data Analysis
- Analyzed global shipping patterns, identifying North America as the lowest-cost region.
- Determined average shipping cost to USA: $62.26 (with standard shipping at $43.20).
- Established baseline metrics for A/B test simulation.
  
#### Phase 3: Strategic A/B Test Simulation
- Built a Python-based A/B test simulator with 4,000 synthetic visitors.
- Tested hypothesis: "Free Shipping with higher product price increases conversions".
- Control Group (A): $250 product + $43.20 shipping.
- Variant Group (B): $295 product with "Free Shipping".
- Conducted statistical significance testing and sensitivity analysis.

## Skills and Tools Used

#### Technical Skills:
- Data Simulation & Synthetic Data Generation.
- Statistical Analysis & Hypothesis Testing.
- A/B Test Design & Implementation.
- Sensitivity Analysis & Break-even Calculation.
- Data Visualization & Dashboard Creation.

#### Tools & Technologies:
- Excel: Data infrastructure, cost modeling, pivot tables.
- Python: Statistical simulation, data analysis, visualization.
- Pandas & NumPy: Data manipulation and numerical computing.
- Matplotlib & Seaborn: Statistical visualization and dashboard creation.
- Scipy: Statistical significance testing (Chi-squared tests).

## Results with Visualizations
Key Findings from A/B Test Simulation:
- Conversion Rate Lift: Variant group showed 35.7% higher conversion (2.45% vs 1.80%).
- Profitability Impact: Variant group generated 40% higher total profit ($3,518 vs $2,520).
- Statistical Context: P-value of 0.193 indicated trend but not 95% significance in this simulation.
- Break-even Analysis: Strategy becomes profitable at 2.04% conversion rate - below achieved rate.

## Visualization Highlights:
![Image] (ab_test_dashboard.png)

- Conversion Rate Comparison: Bar chart showing 2.45% vs 1.80% with confidence intervals.
- Profit per Visitor: Visualization demonstrating $1.76 vs $1.26 advantage for variant group.
- Statistical Summary: Table showing key metrics and significance testing results.
- Sensitivity Analysis: Chart revealing profitability across different conversion scenarios.

## Critical Insight from Sensitivity Analysis:

![Image] (sensitivity_analysis_dashboard.png)

The "Free Shipping" strategy maintained profitability across a wide range of conversion rates, demonstrating low risk and high potential upside.

## Concluding Business Recommendation

### Implementation Recommendation:
Adopt the "Free Shipping" strategy (Variant B) for Sole Capsule's US market launch.
Strategic Rationale:
1.	Profitability Evidence: The variant group showed 40% higher total profit despite smaller sample size.
2.	Low Risk Profile: Sensitivity analysis confirms profitability even with minimal conversion lifts.
3.	Competitive Advantage: "Free Shipping" is a proven conversion driver in e-commerce.
4.	Customer Psychology: Eliminating surprise shipping costs reduces cart abandonment.

Next Steps for Implementation:
1.	Launch Strategy: Implement $295 "all-inclusive" pricing for US customers at launch.
2.	Performance Monitoring: Track conversion rates, average order value, and customer acquisition cost.
3.	Carrier Optimization: Continue analyzing actual shipping costs for carrier negotiation.
4.	Geographic Expansion: Apply similar analysis framework to European markets post-US launch.
5.	Live A/B Testing: Conduct formal A/B tests once sufficient traffic is available.

Risk Mitigation:
- Maintain flexibility to adjust pricing if conversion targets aren't met.
- Monitor carrier performance to ensure shipping cost assumptions remain valid.
- Gather customer feedback on pricing perception and shipping expectations.
