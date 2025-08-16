# PMGSY Scheme Analysis (SQL Project)

## 📌 Project Overview
This project analyzes the **Pradhan Mantri Gram Sadak Yojana (PMGSY)** scheme dataset using SQL.  
The dataset contains information about **sanctioned and completed road works, bridges, road lengths, expenditure, and utilization** across multiple states and schemes.  

The goal of this project is to track the progress of rural road development and identify areas where completion rates or fund utilization need improvement.

---

## 📂 Dataset
- **File**: `pmgsy_scheme.csv`  
- **Source**: Government data (imported as CSV into MySQL),(www.data.gov.in)
- **Key Columns**:
  - `state_name`
  - `district_name`
  - `pmgsy_scheme`
  - `no_of_road_works_sanctioned`
  - `no_of_road_works_completed`
  - `length_sanctioned_km`
  - `length_completed_km`
  - `no_of_bridge_works_sanctioned`
  - `no_of_bridge_works_completed`
  - `cost_sanctioned_lakhs`
  - `expenditure_lakhs`

---

## ⚙️ SQL Queries Performed
✔️ State-wise and scheme-wise progress tracking  
✔️ Road completion percentage calculation  
✔️ Expenditure vs sanctioned cost utilization  
✔️ Pending road works and pending road length  
✔️ Bridge construction analysis  
✔️ District-level breakdown (example: Odisha)  

👉 All queries are stored in [`PMGSY_analysis.sql`](./PMGSY_analysis.sql).

---

## 📊 Key Insights
- States with **highest road completion percentage**  
- States where **expenditure utilization is low** compared to sanctioned funds  
- **Pending works and lengths** highlighting backlog areas  
- **Scheme-wise performance comparison** (PMGSY-I, II, III, PM-JANMAN, etc.)  

---

## 🚀 How to Run
1. Import the dataset into MySQL:
   ```sql
   LOAD DATA INFILE 'path_to_file/pmgsy_scheme.csv'
   INTO TABLE pmgsy_scheme
   FIELDS TERMINATED BY ','
   IGNORE 1 ROWS;


