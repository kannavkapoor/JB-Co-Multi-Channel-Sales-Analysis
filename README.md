JB&Co Multi-Channel Sales Analysis (Power BI)

An interactive Power BI dashboard designed to analyze and visualize multi-channel sales data from **Amazon**, **Flipkart**, **Retail**, and **Wholesale** platforms.  
This project was completed as part of a **Data Analyst Skill Test for JB&Co**, using **sample sales data** to demonstrate data cleaning, modeling, and visualization skills.

---

🎯 Objective
The goal of this project was to clean, organize, and visualize sales data from multiple channels to:
- Identify top-performing products and platforms  
- Track revenue and unit sales trends  
- Generate actionable insights to improve marketing and sales strategies  

---

🧹 Data Cleaning & Preparation
Data cleaning and ETL were performed in **Power Query** within Power BI:
- Removed duplicates and standardized product names  
- Checked and handled missing values  
- Verified correct data types (dates, numbers, text)  
- Ensured correct alignment between *Revenue*, *Discount*, and *Units Sold* fields  

---

🔗 Data Consolidation
- Combined three separate datasets (**Amazon**, **Flipkart**, **Retail & Wholesale**) into one master file  
- Added a new column **“Sales Channel”** to identify each record’s source  
- Created relationships in Power BI for seamless cross-channel analysis  

---

📊 Visualizations
The dashboard was designed across **three continuous pages**:
1. **Overview Dashboard** – KPIs showing Total Revenue, Total Units Sold, and Channel Contribution  
2. **Channel Analysis** – Comparison of revenue by Amazon, Flipkart, Retail, and Wholesale  
3. **Product Insights** – Product-wise revenue, daily sales trends, and top SKUs  

Key Visuals Used
- Line chart for daily sales trends  
- Bar and column charts for revenue by channel/product  
- KPI cards for quick stats  
- Slicers for channel-based filtering  
- Funnel chart for top-performing products  

---

🧮 DAX Measures (Examples)
```DAX
Total Revenue = SUM(Sales[Revenue])
Total Units Sold = SUM(Sales[Units Sold])
Profit Margin = DIVIDE(SUM(Sales[Revenue]) - SUM(Sales[Discount]), SUM(Sales[Revenue]))
