# Credit-Card-Insights-and-Customer-Analysis-PowerBI
“Power BI dashboards analyzing credit card performance &amp; customer profiles using PostgreSQL and CSV data.”
# Credit-Card-Customer-Analytics-PowerBI

## 📌 Project Overview  
This Power BI project provides a **complete 360° analysis** of **Credit Card Customers** and **Credit Card Transactions**, created by connecting Power BI directly to **PostgreSQL** and importing cleaned CSV datasets.

The dashboard helps businesses understand:

- Total revenue generated  
- Interest earned  
- Customer satisfaction  
- Demographics (age, gender, education, job)  
- Credit card usage patterns  
- Spending trends by category  
- Income-based segmentation  
- Quarterly revenue insights  

This is a **real-world banking analytics project** that covers both **Customer Profiling** and **Credit Card Performance**.

---

## 🔗 Data Source (PostgreSQL)
This project uses **PostgreSQL Database** as backend:

- Tables used:
  - `public.cc_detail` → Credit card transaction table  
  - `public.cust_detail` → Customer demographic table  
- Connection established via:
  - **Power BI → Get Data → PostgreSQL Database**

---

## 📁 Files Included  
| File Name | Description |
|----------|-------------|
| `Credit_Card_Customer_Report.pbix` | Full Power BI Report |
| `credit_card.csv` | Credit Card Transaction Data |
| `customer.csv` | Customer Profile Data |
| `dashboard_credit.png` | Credit Card Dashboard screenshot |
| `dashboard_customer.png` | Customer Report screenshot |
| `README.md` | Project documentation |

> *(Rename screenshots according to your final file names)*

---

## 🖼 Dashboard Previews  
### **Credit Card Report**
![Credit Card Dashboard](dashboard_credit.png)

### **Customer Report**
![Customer Dashboard](dashboard_customer.png)

---

## 🚀 **Key Features**
### **🔹 Credit Card Report**
- Total Revenue: **55M**  
- Total Interest Earned: **8M+**  
- Income Generated: **576M**  
- Customer Satisfaction Score (CSS): **3.19**  
- Revenue segmented by:
  - Gender  
  - Age Group  
  - Customer Job  
  - Education Level  
  - Regions & States  
- Total Transactions by quarter  
- High-Level Revenue Trend Analysis (Year → Quarter → Month → Week → Day)

---

### **🔹 Customer Profile Report**
- Customer demographics:
  - Age  
  - Gender  
  - Education Level  
  - Marital Status  
  - Job Type  
- Loan ownership breakdown (car loan, house loan, personal loan)
- Income distribution across customer segments
- Satisfaction scoring analysis
- State-wise top customers
- Spending behavior by expense type:
  - Travel  
  - Grocery  
  - Entertainment  
  - Fuel  
  - Bills  

---

## 🛠 Tools & Technologies Used  
- **Power BI Desktop**  
- **PostgreSQL Database**  
- **SQL Queries** (for cleaning & transformation)  
- **DAX Measures**  
- **Power Query**  
- **CSV Files**  

---

## ⭐ Sample DAX Measures  
```DAX
Total Revenue = SUM(cc_detail[Total_Trans_Amt])

Total Interest Earned = SUM(cc_detail[Interest_Earned])

CSS Score = AVERAGE(cust_detail[Cust_Satisfaction_Score])

Quarterly Revenue = CALCULATE([Total Revenue], VALUES(cc_detail[Qtr]))
```

---

## 🎯 Insights From Analysis (Business Insights)
- Female customers generate slightly **higher revenue** in Q4  
- Highest spending occurs on **Grocery, Bills, and Travel**  
- **Blue Card** category is used by majority customers  
- Age group **30–40** contributes highest transaction volume  
- **Self-employed & White-collar** jobs drive the maximum revenue  
- **TX, NY, CA** are top-performing states  
- Customers using **Swipe** method contribute higher transaction counts  
- Higher Income groups generate **significantly higher revenue**  

---

## 📥 How to Use This Project  
1. Download `.pbix` file  
2. Connect to PostgreSQL (optional — if you want live connection)  
3. Load CSV files if using file-mode  
4. Refresh data  
5. Explore report pages  
   - Credit Card Report  
   - Customer Insights Report  

---

## 📂 Folder Structure  
```
📁 Credit-Card-Customer-Analytics-PowerBI
 ├── 📄 Credit_Card_Customer_Report.pbix
 ├── 📄 credit_card.csv
 ├── 📄 customer.csv
 ├── 📄 dashboard_credit.png
 ├── 📄 dashboard_customer.png
 └── 📄 README.md
```

---

## 🙋 Author  
**Vishal Sharma**

---

## ⭐ Support  
If you find this project useful, please ⭐ **star the repository**  
