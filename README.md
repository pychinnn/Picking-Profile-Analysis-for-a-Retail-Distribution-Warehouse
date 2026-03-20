# Retail Distribution Warehouse: Outbound Fulfilment Optimization

## Executive Summary
This project analyses the outbound operations of a recently acquired Retail Distribution Warehouse during a 3-month transitional period. This warehouse is facing a critical **79% non-fulfilment rate**, the objective was to utilize data analytics to identify operational bottlenecks, simulate process improvements, and design a phased turnaround strategy to stabilize throughput and reduce retail out-of-stock (OOS)) scenarios.

## Key Achievements and Methodologies Used
* **Data Consolidation**: Aggregated raw outbound transaction logs to establish the performance baseline, revealing a critical **79% fulfilment gap**.
* **Process Simulation**: Modelled a transition from "Pick by Order" to "Pick by Product", projecting a 49% reduction in handling frequency.
* **ABC-XYZ Analysis**: Segmented SKUs by volume and demand predictability to design a **pick face allocation strategy**.

## Business Context
The client recently took over operations of a Retail Distribution Warehouse. Due to limited internal familiarity with the outbound process control, the warehouse was struggling to meet basic delivery targets.
* **Problem**: Consistent delivery failures created "inventory gaps" at retail outlets, leading to **lost revenue and inflated cost-to-serve** from redundant logistics attempts.
* **Goal**: Identify the **root causes** of fulfilment failures and implement **measures** to close the gap.

## Data-Driven Insight and Bottleneck Identification
### 1. Overall throughput and operational constraints
* **Observation**: **July 2023** recorded the **highest Order Fulfill Rate (24%)** within the 3-month period. Although total order volume decreased to 8,833 lines, the data indicates a clear **improvement** in operational efficiency compared to June 2023.
* **Bottleneck**: The **79% non-fulfillment** rate remains significantly **below industry benchmarks** for retail logistics.
* **Insight**: These consistent delivery failures created "**inventory gaps**" at retail outlets. This leads to chronic **out of stock (OOS) scenarios**, which directly impact the overall **revenue** and increase the **cost to serve** due to repeated, unsuccessful logistics attempts.
<img width="1357" height="549" alt="image" src="https://github.com/user-attachments/assets/856f46f2-ae51-4fa2-b0f7-42c76cd2bf71" />

### 2. Labour Allocation
* **Observation**: **July** data shows a **shift in demand patterns** compared to the 3-month average. Monday and Saturday have emerged as the **primary high-volume days**, while the overall fulfillment rate has stabilized.
* **Bottleneck**: **Sunday** remains the **lowest** demand day, yet it continues to consume **operational overhead and labour hours** without generating significant output.
* **Insight**: Maintaining **full operations** on Sunday is inefficient. The labour schedule should **align with the actual demand peaks** on Monday and Saturday.
<img width="1182" height="549" alt="image" src="https://github.com/user-attachments/assets/cc03df78-9424-4328-8899-53e3cd3026bc" />


### 3. Category-Specific Performance Failure
* **Observation**: Fulfillment performance is vaires drastically by category. "CHILLED & FROZEN" leads with an **83% success rate** (307 of 370 lines), whereas "PHARMACEUTICAL" shows a **critical service failure with only a 6% success rate**. **High-volume categories** such as "GOURMET USE" and "GROCERY" average only **21.5% success rate**, accounting for bulk of unfulfilled demand.
* **Bottleneck**: The failure in "GOURMET USE" (8,898 lines) and "GROCERY" (8,135 lines) is driven by **sheer volume overwhelming the current resources**. Conversely, the "PHARMACEUTICAL" failure to be a process constraint, likely due to specific picking protocols or security requirements.
* **Insight**: The success in "CHILLED & FROZEN" proves that the warehouse can handle a specialized zone well. The issue in "GOURMET USE" and "GROCERY" is a **scalability**, while the issue in "PHARMACEUTICAL" is **process**. The high volume is currently being sacrificed due to the lack of a specialized **high-density picking strategy**.
<img width="1182" height="563" alt="image" src="https://github.com/user-attachments/assets/2ffbe365-9f59-4b22-9046-9a31ef16ecaa" />


### 4. Picking Process Simulation: "Pick by Order" vs "Pick by Product"
* **Observation**: By simulating an "Pick by Product" model, the total Handling Frequency is **reduced by 49%** (droppig from 63,307 to 32,289 touches).
* **Bottleneck**: The current "Pick by Order" is **highly inefficient for high-velocity items**. It forces pickers to visit the **same location multiple times** for different orders, resulting in **redundant travel**.
* **Insight**: The efficiency gain from consolidation outweighs the additional time required for sorting at the dock. This trade-off significantly **optimize both labour hours and MHE (Material Handling Equipment) usage**.
<img width="790" height="589" alt="image" src="https://github.com/user-attachments/assets/b87c3dbf-73d4-400e-ab85-1ac3fa8ae576" />


### 5. Inventory Segmentation (ABC-XYZ Analysis)
* **Observation**: The warehouse maintains a very lean "A-Class" core with only 42 items (23%) driving the majority of revenue. Within this group, 38 items ("AX" and "AY") are relatively **stable and predictable**. However, the largest concentration of SKUs is in the "CZ" category (44 items) are **low volume and unpredictable**.
* **Bottleneck**: Holding more "CZ" items (44) than the entire "A-Class" items (42) means that the picking team is likely **spending as much time navigating around "slow-movers"** as they are managing the products tdrive revenue.
* **Insight**: The high success rate of "A" and "B" items in the stable "X" and "Y" categories suggests that the fulfillment failure is likely not a forecasting issue. The 44 "CZ" items are likely creating **operational noise**, cluttering the warehouse and slowing down the access to the 42 "A" items.
<img width="680" height="572" alt="image" src="https://github.com/user-attachments/assets/f332048d-6a4e-4cbd-a051-0d0e3c74a38c" />


## Recommendations
Based on the data analysis, I proposed the following phased turnaround strategy to the client:
### Phase 1: Quick Wins
1. **Labour realignment**: Suspend active outbound operations on Sundays to eliminate overhead waste and reallocate resources to support weekday peaks. Or utilize Sunday shifts for strategic pre-picking and replenishment.
2.  **High density picking model**: Shift the "Pick by Order" to "Pick by Product" to resolving the volume-based process failures identified in high-velocity categories like "GOURMET USE" and "GROCERY".
3.  **Protocol standardization and training**: Provide a protocol training to ensure the staff fully understand the new protocol.

## Phase 2: Efficiency Audit
1. **Time and motion study**: Conduct a formal study on the picking process to **identify residual bottlenecks** in picking process or travel paths.
2. **Root cause deep dive**: Verify if the fulfilment gap has been closed and identify any remaining **"hidden" constraints**.

## Phase 3: Structural Optimization
1. **Dynamic slotting strategy**: Relocate 38 high-velocity and predictable SKUs (AX/AY) to the **"Nearest to Dispatch" zone** to minimize travel distance for the majority of daily revenue. ABC-XYZ Analysis and SKUs relocation is required to be executed **quarterly**. 

*Note: The data in this repository has been anonymized to protect client confidentiality.*
