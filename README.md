# Revenue Pipeline Control

## **Project Overview**

**The Chaos on the Ground:** Sales teams were fighting a 49% drop-off in the late-stage funnel. Lacking visibility into price elasticity and regional top-performer tactics, leadership was struggling to protect Q4 margins from unnecessary discounting.
**The Solution:** I engineered a high-fidelity pipeline "Control Tower" in Tableau. This actionable monitor exposed the specific conversion bottlenecks and mapped top-agent behaviors across the network, providing a data-backed roadmap to stabilize win rates and enforce pricing integrity.

## **Data Sources**

- **CRM Export Logs (`CRM_dataset.zip`):** Raw, multi-table structural data directly from Salesforce, encompassing Deal status, Account demographics, Agent assignments, and Product lines.

## **Process**

- **Data Engineering:** Replaced manual forecasting by joining Opportunity and Agent ID tables to build a unified analytical source of truth.
- **KPI Programmatic Logic:** Engineered dynamic calculated fields to continuously compare actual closing prices against baseline targets, exposing value positioning gaps.
- **Interactive Control Tower:** Deployed an interactive Tableau dashboard to track pipeline volume against a 48-day average deal cycle and a 51% baseline win rate.

## **Key Findings**

- **Funnel Bottleneck:** Identified a critical **49% drop-off** specifically in the late-stage funnel (transitioning from engaging to closing), mapping the exact point of execution failure.
- **Agent Benchmarking:** Isolated a top-performing anomaly (Agent Darcel Schlecht) who actively outperformed the company baseline by **60%**.
- **Pricing Elasticity:** Highlighted specific product lines suffering from frequent, unnecessary Q4 discounting, directly eroding peak revenue generation ($3.09M in Q2).

## **Recommendations (Operational Scripts)**

- **Sales Optimization Roadmap:** Reverse-engineer Darcel’s "Ideal Closing Script" and mandate its replication across laggard regions to patch the 49% late-funnel leak.
- **Q4 Margin Protection:** Implement strict approval gates for discount triggers in Q4, protecting the pricing integrity of the **GTX Pro** category leader.
- **Positioning Pivot:** Execute a rapid re-evaluation of "MG Special" marketing campaigns in historically underperforming sectors.

## **Next Steps**

- **Golden Pipeline Maintenance:** Automate the CRM data extraction process to feed straight into Tableau via API, eliminating the `.csv` zip export delay.
- **Proactive Alerting:** Configure Tableau threshold alerts to instantly notify regional directors when an active deal stalls past the 48-day cycle average.
