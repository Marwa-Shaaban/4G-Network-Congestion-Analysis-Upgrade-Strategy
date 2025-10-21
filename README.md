# 4G Network Congestion Analysis & Upgrade Strategy

## Project Overview

This project presents a comprehensive analysis of 4G network traffic data for an urban area (Milan). The primary objective is to diagnose the root causes of network congestion, identify spatial and temporal patterns, and propose a data-driven, cost-effective radio upgrade strategy. This was completed as a technical assignment for a role in the telecommunications industry.

---

## Problem Statement

A mobile network operator is facing escalating customer complaints regarding poor data speeds. Before committing to large-scale 5G deployment, the company seeks to maximize the ROI from its existing 4G infrastructure through strategic, targeted upgrades.

---

## Dataset

The analysis was performed on a public dataset representing one week of telecommunications activity in Milan, spatially aggregated into a 100x100 grid with data recorded at 10-minute intervals.

---

## Methodology & Analysis

The project followed a structured, three-part methodology:

### Part A: Temporal & Spatial Analysis
1.  **Data Processing:** Loaded and aggregated 7 days of raw data by timestamp and grid location (`SquareID`).
2.  **Temporal Analysis:** Analyzed traffic patterns to identify the network's overall **Busy Hour**.
3.  **Spatial Analysis:** Calculated total traffic for each grid square to identify the **Top 10 Hotspots** and visualized the spatial distribution using a heatmap.

### Part B: Root Cause Diagnosis
1.  **Capacity Utilization:** Calculated the capacity utilization percentage for the hotspots during the busy hour, using a baseline of a 150 Mbps sector capacity.
2.  **Correlation Analysis:** Assessed the relationship between internet traffic and voice/SMS traffic to diagnose the problem type.

### Part C: Strategic Upgrade Plan
1.  **Solution Portfolio:** Defined a set of hardware and software solutions to address the diagnosed issues.
2.  **Phased Rollout:** Organized the solutions into a strategic 3-phase implementation plan that balances cost and impact.

---

## Key Findings & Results

* **Busy Hour:** The network busy hour was identified at **17:00 (5 PM)**.
* **Top 10 Hotspots:** The analysis successfully identified the 10 specific grid squares with the highest data traffic load.
* **Root Cause:** The diagnosis definitively concluded that the issue is **Capacity Exhaustion**. The top hotspots operate at up to **95.5%** of their maximum capacity.
* **Correlation:** The analysis showed **significant correlation** between data and voice/SMS traffic.

---

## Proposed Solution: A 3-Phase Upgrade Strategy

A strategic plan was developed to address the capacity limitations effectively:

| Phase                  | Recommended Actions                                                               | Target Areas        |
| :--------------------- | :-------------------------------------------------------------------------------- | :------------------ |
| **Phase 1: Quick Wins**| • Implement Load Balancing<br>• Optimize QoS Parameters                              | All 10 Hotspots     |
| **Phase 2: Targeted Upgrades**| • Activate Carrier Aggregation (CA)<br>• Upgrade antennas to 4x4 MIMO            | Top 5 Hotspots      |
| **Phase 3: Long-Term Solution**| • Implement Sector Splitting                                                      | Top Hotspot Only    |

This phased approach ensures the best Return on Investment (ROI) by prioritizing low-cost software optimizations before committing to targeted hardware upgrades.

---

## Tools Used

* **Programming Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Plotly
* **Environment:** Jupyter Notebook

---

## How to View This Project

* The complete step-by-step analysis, code, and visualizations can be found in the **Jupyter Notebook (`.ipynb`) file**.
* A high-level summary of the findings and the final strategic plan is available in the **PowerPoint Presentation (`.pptx`) file**.
