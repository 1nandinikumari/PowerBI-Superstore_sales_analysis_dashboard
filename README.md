# 📊 **Superstore Sales Analysis – Power BI**

## 📌 **Project Overview**
This project analyzes **Superstore sales data** using **Power BI** to evaluate sales performance, profitability, regional trends, and short-term sales forecasting.  
The dashboard transforms raw data into **interactive business insights** using data modeling and DAX.

---

## 🎯 **Objective**
- Analyze **Sales, Profit, Quantity, and Delivery Trends**
- Compare performance across **Regions, Categories, and Segments**
- Identify **Top States by Sales and Profit**
- Build a **15-Day Sales Forecast** using historical data

---

## ⚙️ **Key Steps**
- Data cleaning and validation in Power BI  
- Data modeling using star schema  
- Created calculated measures using **DAX**  
- Grouped regions using **SWITCH DAX logic**  
- Implemented **sales forecasting**

---

## 🧮 **DAX Used (Example)**
```DAX
Region Group =
SWITCH(
    TRUE(),
    Orders[Region] IN {"Central US","Eastern US","Southern US","Western US"}, "America",
    Orders[Region] IN {"Central Africa","Eastern Africa","Southern Africa","Western Africa"}, "Africa",
    Orders[Region] IN {"Central Asia","Eastern Asia","Southeastern Asia","Southern Asia","Western Asia","Oceania"}, "Asia Pacific",
    Orders[Region] IN {"Eastern Europe","Northern Europe","Southern Europe","Western Europe"}, "Europe",
    "Other"
)
```
---

## **🔍 Key Insights**

-Technology category generates highest sales
-Consumer segment drives maximum revenu
-Some regions have high sales but lower profit margins
-Forecast shows stable short-term sales trend

---

## **🛠️ Tools & Technologies**

-Power BI
-DAX
-Power Query
-Data Modelin
-Forecasting
