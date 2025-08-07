
# 🧩 Customer Segmentation

This project focuses on customer segmentation using the RFM (Recency, Frequency, Monetary) model. SQL Server was used for data processing and segmentation logic, while Power BI was used to build an interactive dashboard for business analysis.

---

## 🧠 Project Objectives

- Segment customers based on RFM scores
- Identify high-value and at-risk customer groups
- Visualize distribution and cumulative contribution of customer groups
- Support marketing and retention strategies through data insights

---

## 🛠️ Workflow Summary

### 🗃️ Data Processing – SQL Server

Customer transactions were processed using SQL to compute RFM values:

- Recency: Days since last transaction
- Frequency: Number of unique transactions
- Monetary: Total GMV (Gross Merchandise Value)
- Customers were ranked into 4 quantiles for each R, F, and M dimension using NTILE(4)
- Final RFM score was built as a concatenated 3-digit value (e.g., 444, 321)

---

### 📊 Data Visualization – Power BI

Power BI was used to:

- Visualize customer group distribution by RFM
- Show contribution to revenue and volume by segment
- Calculate cumulative revenue and customer ratios using DAX
---

## 🗝️ Key Insights
- Group 444 (recent, frequent, high-spending customers) is the most profitable segment, contributing nearly 22% of total revenue.

- Groups 112 and 214, despite previously generating high revenue, have not made recent or frequent purchases — suggesting that the product may no longer fully meet their needs.

- Around 60% of customers fall within just one-third of RFM combinations, reflecting a strong concentration of recurring behavioral patterns.

- General Customers represent the largest share in both customer count and revenue (~29.4%), but exhibit price sensitivity despite frequent purchases.

- VIP Customers, although only 16.5% of the base, contribute over 27% of total revenue due to high purchase frequency and transaction value.

- Secondary Customers are less active but still contribute ~2.7 billion in revenue — posing a significant churn risk and should be targeted for reactivation.

- Potential Customers are regular buyers with moderate-to-high order values and show clear potential to be upgraded to VIPs through incentives or loyalty programs.

- The RFM segmentation reveals actionable opportunities to retain VIPs, reactivate dormant segments, and nurture price-sensitive but loyal customers for sustainable revenue growth.

---

## 📁 Project Files  

| File / Folder | Description |
|---------------|-------------|
| [Query & DAX](https://github.com/ntmh12/customer-segmentation/blob/main/Query%20%26%20DAX.txt) | Contains full SQL and DAX logic |
| [visualization/Dashboard.png](https://github.com/ntmh12/customer-segmentation/blob/main/visualization/Dashboard.png) | Preview image of the Power BI dashboard |
| [visualization/Dashboard.pbix](https://github.com/ntmh12/customer-segmentation/blob/main/visualization/Dashboard.pbix) | Full interactive Power BI dashboard file |
| [Customer Report.pdf](https://github.com/ntmh12/customer-segmentation/blob/main/Customer%20Report.pdf) | Final report |
| `README.md` | Project documentation |

---

## 🧰 Tools & Technologies

- **SQL Server**: Transaction data extraction and RFM grouping
- **Power BI**: Data visualization and DAX
