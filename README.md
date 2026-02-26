# Retail Distribution Warehouse: Outbound Fulfillment Optimization

## Executive Summary
This project analyses the outbound operations of a recently acquired Retail Distribution Warehouse during a 3-month transitional period. This warehouse is facing a critical **79% non-fulfilment rate**, the objective was to utilize data analytics to identify operational bottlenecks, simulate process improvements, and design a phased turnaround strategy to stabilize throughput and reduce retail out-of-stock (OOS)) scenarios.

## Key Achievements and Methodologies Used
* **Data Consolidation**: Aggregated raw outbound transaction logs to establish the performance baseline, revealing a critical **79% fulfillment gap**.
* **Process Simulation**: Modeled a transition from "Pick by Order" to "Pick by Porduct", projecting a 49% reduction in handling frequency.
* **ABC-XYZ Analysis**: Segmented SKUs by volume and demand predictability to design a **pick face allocation strategy**.

## Business Context
The client recently took over operations of a Retail Distribution Warehouse. Due to limited internal familarity with the outbound process control, the warehouse was struggling to meet basic delivery targets.
* **Problem**: Consistent delivery failures created "inventory gaps" at retail outlets, leading to **lost revenue and inflated cost-to-serve** from redundant logistics atempts.
* **Goal**: Identify the **root causes** of fulfilment failures and implement **measures** to close the gap.

## Data-Driven Insight and Bottleneck Identification
### 1. Overall throughput and operational constraints
* **Observation**: The order **fulfilment rate** peaked at only **24%** in July 2023 (despite the total transactions drop to 8,833 lines).
* **Bottleneck**: The warehouse is physically constrained to a maximum of **~75 successful transactions per day**.
* **Insight**: The 79% non-fulfilment rate falls drastically below retail logistics benchmarks.

### 2. Labour Allocation
* **Observation**: July data reveals **Monday** and **Saturday** as peak demand days. Conversely, Sunday is the lowest demand day.
* **Bottleneck**: Maintaining full operations on Sundays consumes overhead and labour without generating significant output.
* **Insight**: Labour scheduling is misaligned with actual throughput demands.

### 3. Category-Specific Performance Failure
* **Observation**: Fulfilment varies drastically by zone. "CHILLED & FROZEN" leads with an 83% success rate. However, "GOURMET USE" and "GROCERY" average a 21.5% success rate, and "PHARMACEUTICALS" shows a critical faiure at 6%.
* **Bottleneck**: "GOURMET USE" (8,898 lines) and "GROCERY" (8,135 lines) are failing due to sheer volume overwhelming current resources. "PHARMACEUTICALS" is failing due to process constraints (likely picking protocols).
* **Insight**: The warehouse can successfully manage specialized zone (CHILLED & FROZEN), but lasks a high-density picking strategy for bulk categories.

### 4. Picking Process Simulation: "Pick by Order" vs "Pick by Product"
* **Result**: The current "Pick by Order" method forcess pickers into redundant travel paths for high-velocity items.
* **Bottleneck**: The labour and MHE efficiency gained from batch picking outweighs the minimal extra time needed for dock-sorting.

### 5. Inventory Segmentation (ABC-XYZ Analysis)
* **Observation**: A lean "A-Class" core of just 42 items (23%) drives the majority of revenue, with 38 of these are being highly predictable (AX and AY). Meanwhile, the warehouse holds 44 "CZ" items (low volume and highly unpredictable).
*  **Bottleneck**: Pickers spend excessive time navigating around "slow
