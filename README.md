
# 🧩 Customer Segmentation with SQL & Power BI

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

## 📁 Project Structure

| File / Folder | Description |
|---------------|-------------|
| `[Query & DAX.txt](https://github.com/ntmh12/customer-segmentation/blob/main/Query%20%26%20DAX.txt)` | Contains full SQL and DAX logic |
| `[visualization/Dashboard.png](https://github.com/ntmh12/customer-segmentation/blob/main/visualization/Dashboard.png)` | Preview image of the Power BI dashboard |
| `[visualization/Dashboard.pbix](https://github.com/ntmh12/customer-segmentation/blob/main/visualization/Dashboard.pbix)` | Full interactive Power BI dashboard file |
| `[Customer Report.pdf](https://github.com/ntmh12/customer-segmentation/blob/main/Customer%20Report.pdf)` | Final report |
| `README.md` | Project documentation |

---

## 🧰 Tools & Technologies

- **SQL Server**: Transaction data extraction and RFM grouping
- **Power BI**: Data visualization and DAX modeling
- **DAX**: Cumulative and ratio calculations
- **GitHub**: Documentation and version control

---

## 📬 Contact
 
💼 [LinkedIn](https://www.linkedin.com/in/nguyen-thi-minh-huong/)

---
