# Retail Distribution Warehouse: Outbound Fulfilment Optimization

## Executive Summary
This project analyzes the outbound operations of a recently acquired Retail Distribution Warehouse during a 3-month transitional period. This warehouse is facing a critical **79% non-fulfilment rate**, the objective was to utilize data analytics to identify operational bottlenecks, simulate process improvements, and design a phased turnaround strategy to stabilize throughput and reduce retail out-of-stock (OOS)) scenarios.

## Key Achievements and Methodologies Used
* **Data Consolidation**: Aggregated raw outbound transaction logs to establish the performance baseline, revealing a critical **79% fulfilment gap**.
* **Process Simulation**: Modelled a transition from "Pick by Order" to "Pick by Product", projecting a 49% reduction in handling frequency.
* **ABC-XYZ Analysis**: Segmented SKUs by volume and demand predictability to design a **pick face allocation strategy**.

## Business Context
The client recently took over operations of a Retail Distribution Warehouse. Due to limited internal familiarity with the outbound process control, the warehouse was struggling to meet basic delivery targets.
* **Problem**: Consistent delivery failures created "inventory gaps" at retail outlets, leading to **lost revenue and inflated cost-to-serve** from redundant logistics atempts.
* **Goal**: Identify the **root causes** of fulfilment failures and implement **measures** to close the gap.

## Data-Driven Insight and Bottleneck Identification
### 1. Overall throughput and operational constraints
* **Observation**: The order **fulfilment rate** peaked at only **24%** in July 2023 (despite the total transactions drop to 8,833 lines).
* **Bottleneck**: The warehouse is physically constrained to a maximum of **~75 successful transactions per day**.
* **Insight**: The 79% non-fulfilment rate falls drastically **below retail logistics benchmarks**.
<img width="1357" height="549" alt="image" src="https://github.com/user-attachments/assets/856f46f2-ae51-4fa2-b0f7-42c76cd2bf71" />

### 2. Labour Allocation
* **Observation**: July data reveals **Monday** and **Saturday** as peak demand days. Conversely, Sunday is the lowest demand day.
* **Bottleneck**: Maintaining full operations on Sundays **consumes overhead and labour** without generating significant output.
* **Insight**: Labour scheduling is **misaligned** with actual throughput demands.
<img width="1182" height="549" alt="image" src="https://github.com/user-attachments/assets/cc03df78-9424-4328-8899-53e3cd3026bc" />


### 3. Category-Specific Performance Failure
* **Observation**: Fulfilment varies drastically by zone. "CHILLED & FROZEN" leads with an 83% success rate. However, "GOURMET USE" and "GROCERY" average a **21.5% success rate**, and "PHARMACEUTICALS" shows a **critical faiure at 6%**.
* **Bottleneck**: "GOURMET USE" (8,898 lines) and "GROCERY" (8,135 lines) are failing due to **sheer volume overwhelming current resources**. "PHARMACEUTICALS" is failing due to process constraints (likely picking protocols).
* **Insight**: The warehouse can successfully manage specialized zone (CHILLED & FROZEN), but **lasks a high-density picking strategy** for bulk categories.
<img width="1182" height="563" alt="image" src="https://github.com/user-attachments/assets/2ffbe365-9f59-4b22-9046-9a31ef16ecaa" />


### 4. Picking Process Simulation: "Pick by Order" vs "Pick by Product"
* **Result**: Modeling a "Pick by Product" approach reduced total Handling Frequency by **49%** (dropping from 63,307 to 32,289 touches). 
* **Bottleneck**: The current "Pick by Order" method forces pickers into **redundant travel paths** for high-velocity items.
* **Insight**: The labour and MHE efficiency gained from batch picking vastly outweighs the **minimal extra time** needed for dock-sorting.
<img width="790" height="589" alt="image" src="https://github.com/user-attachments/assets/b87c3dbf-73d4-400e-ab85-1ac3fa8ae576" />


### 5. Inventory Segmentation (ABC-XYZ Analysis)
* **Observation**: A lean "A-Class" core of just **42 items (23%) drives the majority of revenue**, with 38 of these are being highly predictable (AX and AY). Meanwhile, the warehouse holds **44 "CZ" items (low volume and highly unpredictable)**.
*  **Bottleneck**: Pickers spend **excessive time navigating around "slow-movers" (CZ)** to access revenue-driving items.
*  **Insight**: The fulfilment gap is operational. Slow movers are creating **operational noise and clutter**.
<img width="680" height="572" alt="image" src="https://github.com/user-attachments/assets/f332048d-6a4e-4cbd-a051-0d0e3c74a38c" />


## Recommendations
Based on the data analysis, I proposed the following phased turnaround strategy to the client:
### Phase 1: Quick Wins
1. **Labour realignment**: Suspend Sunday outbound operations and **reallocate the resources to high-volume peaks (Monday or Saturday)**. Or utilize Sunday for **strategic pre-picking and replenishment**.
2.  **High density picking model**: Transition from "Pick by Order" to "Pick by Product" for **high-velocity categories**.
3.  **Protocol standardization and training**: Deploy specialized **training for the new Picking by Product workflow** to ensure process compliance.

## Phase 2: Efficiency Audit
1. **Time and motion study**: Conduct a formal study on the picking process to **identify residual bottlenecks** in picking process or travel paths.
2. **Root cause deep dive**: Verify if the fulfilment gap has been closed and identify any remaining **"hidden" constraints**.

## Phase 3: Structural Optimization
1. **Dynamic slotting strategy**: Relocate 38 high-velocity and predictable SKUs (AX/AY) to the **"Nearest to Dispatch" zone** to minimize travel distance for the majority of daily revenue. ABC-XYZ Analysis and SKUs relocation is required to be executed **quarterly**. 

*Note: The data in this repository has been anonymized to protect client confidentiality.*
