# Revenue Pipeline Control & Funnel Analytics
#### Business Intelligence Engineering | Advanced Tableau | Funnel Analysis | Executive Dashboards

[![Tableau](https://img.shields.io/badge/Tableau-Advanced_Dashboard_Engineering-E97627.svg)](https://www.tableau.com/)
[![Domain](https://img.shields.io/badge/Domain-Business_Intelligence_%26_Analytics-4B0082.svg)](https://en.wikipedia.org/wiki/Business_intelligence)

> [!IMPORTANT]
> **Executive Summary:** This project demonstrates end-to-end BI engineering — from raw pipeline data ingestion to an executive-grade Tableau dashboard for revenue forecasting and conversion funnel analysis. The system replaces manual spreadsheet pipeline reviews with an automated single-source-of-truth that surfaces deal velocity, stage conversion rates, and Win/Loss attribution — enabling a shift from quarterly retrospective analysis to real-time revenue operations.

---


## The Problem

Sales leadership was managing a multi-stage revenue pipeline using static weekly spreadsheet exports — creating a systematic blind spot to intra-week pipeline movement, conversion bottlenecks, and deal velocity anomalies. Strategic decisions were made on lag-delayed data rather than current operational reality.

**Goal:** Replace static reporting with an interactive Tableau-based Revenue Operations Command Center driven by live data modeling, calculated KPIs, and a self-service parameter architecture for scenario planning.

## Data Sources

1. **Primary Dataset:** A synthetic but structurally realistic CRM pipeline export containing Opportunity fields: Stage, Owner, Amount, Close Date, Product, Lead Source.
2. **Additional Data:** Quota targets and Win Rate benchmarks from historical period analysis.

## Process

- **KPI Engineering:** Built calculated fields for Pipeline Velocity, Stage Conversion Rate, Win/Loss Ratio, and Weighted Forecast Value — the primary metrics for revenue operations visibility.
- **Funnel Architecture:** Designed a true sequential conversion funnel (not just a count chart) using LOD expressions to track opportunity movement between stages without inflating pipeline totals.
- **Win/Loss Attribution:** Built a root-cause segmentation view decomposing losses by Stage, Product, Owner, and Lead Source to surface actionable attribution data.
- **Parameter-Driven Forecasting:** Implemented Tableau parameter controls allowing leadership to model "What-If" close rate and ASP scenarios without touching underlying data.

## Technical Pivot

**From Static Snapshots to Live BI Architecture**

The original reporting was entirely based on scheduled CSV exports from the CRM, creating 5–7 day lag windows between events and reporting.
- **The Change:** Restructured the Tableau workbook to consume a live-connected view directly from the data layer, enabling near-real-time pipeline visibility.
- **The Result:** Eliminated data lag and moved the team from weekly retrospective reviews to daily pipeline hygiene conversations — a fundamental shift in operational cadence.

**Calculated Funnel vs. Simple Stage Count**

Common dashboards count opportunities per stage, which inflates upper-funnel numbers when deals skip stages or return from Closed Lost.
- **The Change:** Implemented Tableau LOD expressions to calculate true stage-by-stage conversion rates using the original opportunity set as the denominator.
- **The Result:** Leadership could see the true Opportunity-to-Proposal conversion rate versus what was previously masked by recycled opportunities re-entering the funnel.

## Key Insights

- **Proposal-to-Close Stage Collapse:** The conversion rate cliff was concentrated in the Proposal-to-Negotiation transition — indicating a proposal quality issue, not a prospecting volume problem.
- **Lead Source Attribution Gap:** Digital-sourced leads entered at 3× the volume of outbound leads but converted at 60% the rate once reaching the Demo stage — a data point invisible in flat-count reporting.
- **Deal Velocity Variance:** The P50 deal cycle was 45 days, but P90 deals took 112 days — indicating a bimodal distribution where a segment of deals was being managed on an entirely different cadence without intervention rules.

## Recommendations

- **Pipeline Hygiene Standards:** Enforce CRM update mandates for all opportunities above the Proposal stage to reduce forecast noise from stale data contaminating the weighted pipeline view.
- **Lead Source Routing:** Invest in a differentiated nurture strategy for digital leads, which enter at high volume but require more structured Stage 2 support to match outbound conversion rates.
- **Velocity Threshold Alerts:** Implement automated notifications for deals exceeding the P75 velocity threshold to trigger manager intervention before stalled deals contaminate quarterly close targets.

## Next Steps

- **CRM Integration:** Connect the Tableau workbook to a live CRM API endpoint to replace the CSV export cycle with continuous data refresh.
- **Quota Attainment Overlay:** Add a Quota Pacing layer to project end-of-period attainment based on current pipeline velocity, not point-in-time snapshots.
- **Predictive Win Score:** Integrate a lightweight ML win probability model into the pipeline view to surface at-risk deals displaying known Stage 2 stall patterns.