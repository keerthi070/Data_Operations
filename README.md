# 📊 Data Operations & Validation Pipeline

## 📌 Project Overview
This project demonstrates a **Data Operations workflow** focused on validating, cleaning, and operationalizing large-scale transactional data to generate reliable business reports.  
It mirrors real-world responsibilities such as data quality checks, audit logging, KPI generation, and reporting automation.

---

## 🧾 Dataset Description
- Transactional dataset with **~800,000 records**
- Key fields:
  - `invoice`
  - `stockcode`
  - `description`
  - `quantity`
  - `price`
  - `invoicedate`
  - `customerid`
  - `country`
- Represents raw operational data containing real-world inconsistencies.

---

## ✅ Data Validation Checks
The following quality checks were performed:

- Missing customer IDs  
- Duplicate records  
- Invalid quantities (≤ 0)  
- Invalid prices  

### Validation Summary
- Total records processed: **797,815**
- Missing customer IDs: **0**
- Duplicate rows: **0**
- Invalid quantity records: **18,390 (~2.3%)**
- Invalid price records: **0**

Invalid records were logged separately to maintain **auditability**.

---

## 🧹 Data Cleaning Rules
- Removed records with invalid quantities (≤ 0)
- Retained valid pricing and customer data
- Ensured dataset integrity before KPI computation

These rules reflect standard **business and operational constraints**.

---

## 📈 Metrics & Reporting
After cleaning, the following operational metrics were generated:

- Revenue per transaction  
- Total orders  
- Unique customers  
- Daily total revenue  

A **daily operations report** was created to support business tracking and decision-making.

---

## 📁 Project Outputs
- `daily_operations_report.csv`  
  → Daily KPIs (orders, customers, revenue)
- `invalid_quantity_log.csv`  
  → Audit log of invalid operational records

---

## 🛠 Tools & Technologies
- Python  
- Pandas  
- Jupyter / Google Colab  

---

## 💼 Relevance to Data Operations Role
This project aligns with the responsibilities of a **Data Operations Associate**, including:

- Data collection and validation  
- Quality control and auditing  
- Reporting & documentation  
- Process standardization  
- Automation-ready workflows  

