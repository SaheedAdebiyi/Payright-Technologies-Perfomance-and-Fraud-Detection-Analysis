# Payright-Technologies-Perfomance-and-Fraud-Detection-Analysis
**Author:**  Saheed Olayinka Adebiyi
**Date:** 2025-12-03
---
## Project Background
This analysis was conducted to identify the root causes of these issues and support data-driven strategic decisions due to the recent decline in recently experience in transaction failures, declining approval rates, and increased customer complaints despite sufficient account balances. At the same time, fraud-related chargebacks continue to occur even after an upgrade of the fraud detection system. There are also concerns about the actual performance and value of the bank’s premium 5G network slicing investment. This project analyzes available data and produces an interactive Excel dashboard with actionable recommendations.
---
## Project Objective
The following objectives guide the analysis of platform performance and fraud detection to identify key issues and actionable insights.
**Performance Objectives**
**Identify the root causes of declining approval rates.
Assess mobile vs. desktop performance to guide improvements.
Evaluate the effectiveness of 5G Network Slicing on transaction success.
Detect key performance bottlenecks across the platform.**

**Fraud Detection Objectives*
Determine if flagged fraud is being blocked in real time.
Analyze fraud trends and chargebacks to quantify risk.
Identify gaps in the upgraded fraud system’s accuracy and response.*
---
## Datasets
- **transaction_dataset_JanToOct.xlsx** — The data consists of 40,000 rows and 14 columns, which is clean without duplicates and empty spaces, except for creating new conditional columns
Dataset main columns include: Transaction ID, Sender Account ID, Receiver Account ID, Transaction Amount, Transaction Type, Timestamp, Transaction Status, Fraud Flag, PIN Code, Geolocation, Device Used, Network Slice ID, Latency (ms), and Slice Bandwidth (Mbps)
---
## Dashboard Features
- Key KPIs: total number of transactions, Approval rate, total Fraud Flagged, total fraud blocked, Total chargebacks
- Visuals: volume of transactions by device, count of failed transactions by device, fraud by device, failure by network latency
- Interactivity: slicers/filters for Device used, transaction status
---
## Key Findings (example)
Mobile and Desktop transactions have almost equal volume, but Desktop shows a slightly higher failure count.
Network Slice 2 records the highest overall transaction count, but Slice 1 shows the highest failed transactions, signaling uneven performance.
The monthly trend reveals inconsistent performance, with visible dips in several months, indicating unstable system reliability.
Approval rate is around 80%, meaning 1 in every 5 transactions fails. This is quite high for a financial service.
Latency categories show rising failures as latency increases, especially within the 100–149 ms and 60–99 ms ranges.
Fraud-flagged cases (2,041) are significantly lower than total transactions, yet 397 fraudulent transactions were blocked, showing system gaps.
Mobile and Desktop have almost identical fraud distribution, meaning fraud is not device-dependent.
Fraud attempts are highest in Transfer and Withdrawal transactions, indicating targeted exploitation.
Network Slice analysis shows fraud flags distributed evenly across slices, suggesting fraudsters are not favoring any particular network route.
Fraud trend over time shows spikes in specific months, indicating seasonal or campaign-driven fraud attacks.

---
## Recommendations
1. Implement targeted device-specific improvements, especially for Desktop.
2. Increase approval rate through backend process optimization and faster validation checks.
3. Enhance fraud-scoring algorithms to reduce the number of fraud-flagged = TRUE transactions that still succeeded.
4. Deploy transaction-type-specific fraud rules, especially for Transfers and Withdrawals.
5. Implement an early-warning system for months with historically high fraud peaks.
6. Strengthen behavioral analytics to detect bot-based or repeated fraud attempts across both devices.
7. Introduce multi-layer verification for high-risk transactions with high amounts or unusual patterns.

---
## Tools & Techniques
- Microsoft Excel (Pivot Tables, Pivot Charts, Slicers) 
- Data cleaning and transformation in Excel 
- Dashboard layout and visualization best practices 
- Basic descriptive analytics and KPI design
---
## Project Files (included)
- `transaction_dataset_JanToOct.xlsx` — interactive dashboard file 
- `Payright Performance and fraud detection presentation.pdf` — boardroom slide deck 
- `README.md` — this documentation
---
## How to Run / View
1. Open `transaction_dataset_JanToOct.xlsx` in Excel (desktop recommended) 
2. Enable content (if prompted) to allow Pivot Tables and slicers to work 
3. Use slicers to filter by Device used, transaction status, etc. 
4. Refer to `Payright Performance and fraud detection presentation.pdf` for a summary of insights and recommended actions
---
## Contact
Adebiyi Saheed Olayinka 
Email: olayinkaadebiyi49@gmail.com
LinkedIn: www.linkedin.com/in/olayinkaadebiyi
