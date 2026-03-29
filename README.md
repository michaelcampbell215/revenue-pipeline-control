# Predictive Revenue Pipeline Control

[![Tableau](https://img.shields.io/badge/Tableau-Dashboard-E97627.svg)](https://public.tableau.com/)
[![Analysis](https://img.shields.io/badge/Methodology-Funnel_Analysis-blue.svg)](https://en.wikipedia.org/wiki/Funnel_analysis)

> [!IMPORTANT]
> **Executive Summary:** This project transforms static CRM reporting into a predictive revenue analytics engine. By engineering a dynamic pricing elasticity model, we successfully identified a 49% late-stage funnel leak and isolated the specific negotiation tactics required to protect $3.09M in quarterly revenue margins.

---

## Project Overview

Sales teams were fighting a massive 49% drop-off in the late-stage funnel, and leadership was struggling to protect Q4 margins from unnecessary discounting. Legacy CRM reporting was acting as a static post-mortem tool management had no visibility into real-time price elasticity or exactly why specific deals were dying in the final "Closing" phase.

1. **Description:** We engineered calculated mathematical logic in Tableau to transition the organization from reactive pipeline reporting to forward-looking revenue control.
2. **Objective:** Pinpoint margin leaks *before* the quarter closed, optimize pricing elasticity, and standardize high-performing negotiation behaviors across the entire sales floor.

## Data Sources

1. **Primary Datasets:** Live CRM pipeline exports containing deal stages, expected close dates, expected revenue, and assigned sales agents.
2. **Additional Data:** Historical product pricing baselines to measure explicit margin erosion and exact discounting percentages.

## Process

*   Mapped the entire sales funnel to quantify the exact probability of conversion at each distinct stage, from initial "Engaging" to final "Won."
*   Built mathematical logic to track Sales Velocity ("Days-in-Stage") to identify stagnant deals requiring immediate managerial intervention.
*   Engineered a Pricing Elasticity Index by dynamically comparing actual closing prices against target financial baselines to expose systematic margin erosion.
*   Cross-referenced individual sales agent performance against company-wide baselines to identify behavioral variance.

## Technical Pivot

*   **From Post-Mortem Snapshots to Live Elasticity:** Legacy reporting provided a static snapshot of revenue at the end of the month. We explicitly rejected this architecture. Instead, we engineered calculated logic in Tableau to track **Pricing Elasticity** as a live, fluctuating metric. This transformed the dashboard into an active monitor, pinpointing exactly which products (e.g., GTX Pro) held strong pricing power in the market and which products were suffering from unnecessary, pre-emptive discounting by agents trying to secure volume.

## Key Insights

*   **The 49% Leak Isolated:** The pipeline was healthy at the top of the funnel but collapsing at the final hurdle. Deals were stalling in the final "Closing" phase explicitly due to unstructured discounting practices and weak value positioning.
*   **Performance Anisotropy Exists:** Identified a severe performance gap across the floor. The top-performing agent vastly outperformed the company baseline by 60%, proving that market demand existed if the correct negotiation tactics were applied.
*   **Product-Specific Pricing Power:** Discovered that the high-end "GTX Pro" line maintained extreme pricing elasticity, meaning sales reps could securely hold firm on MSRP without losing the deal, whereas lower-tier products were highly sensitive to absolute price.

## Recommendations

*   **Replicate Top-Performer Tactics:** Reverse-engineer the specific communication methods and email cadences of the top-performing agent to mandate replication across all underperforming sales regions.
*   **Prioritize High-Elasticity Categories:** Shift overall marketing spend and sales focus heavily toward the high-margin GTX Pro line, as the data proves it is highly resistant to competitive margin erosion.
*   **Dynamic Discount Approvals:** Implement data-driven discount triggers inside the CRM that automatically require Director-level executive sign-off when pricing integrity on a specific deal drops below the mathematical tolerance threshold.

## Next Steps & Action Plan

*   **Live Funnel Monitoring:** Equip Regional Directors with real-time dashboard visibility deep into the "Closing" phase to prevent deal stagnation *before* the crucial end of Q4.
*   **Margin Integrity Alerts:** Deploy automated notifications for Sales Directors the very moment regional discounting behavior exceeds the established quarterly tolerance.
