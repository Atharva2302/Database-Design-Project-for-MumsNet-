# MumsNet E-Commerce Database & BI Enhancement Project

This project involved redesigning MumsNet's database system and implementing a Business Intelligence (BI) platform to analyse their online store data using Microsoft SQL Server Analysis Services (SSAS/SSDT). While originally completed as a group project, this repository reflects my **individual contribution** to **Deliverable 2 (D2)**—the complete BI solution.

---

## 📦 Project Structure

```
├── Database/
│   └── D1.bak                 # Full database backup file
├── BI_Solution/
│   └── D2/
│       └── D2.sln            # Visual Studio BI solution file
```

---

## 💼 My Contribution — Business Intelligence Platform (D2)

I developed a full 'proof of concept' BI solution in Microsoft Visual Studio using SSDT and SSAS that fulfilled all core business requirements. This included:

- Creating and configuring **Data Source Views (DSV)**
- Designing **cube dimensions and measures**
- Implementing multiple **hierarchies and KPIs**

---

## 📊 Business Requirements Implemented

### 🛒 Order Analysis
- Number and % of cancelled orders
- Sales value of cancelled orders
- Number and % of unfulfilled basket orders (out-of-stock)
- % of abandoned baskets
- % of fulfilled orders  
> 📌 *All percentages calculated against total orders placed*

---

### 🧭 Hierarchical Analysis

- **Customer Hierarchy**: Customer → City → Region → Country  
- **Product Hierarchy**: Product Variant → Product → Product Group  
- **Time Hierarchy**: Day → Month → Quarter → Year

---

### 📈 Detailed Metrics

- Sales and quantity sold by: Product, Customer, Day
- Ordered stock quantity by: Product, Order Day  
> 📌 *All product metrics are calculated at the variant level*

---

## ⚙️ Technologies Used

- Microsoft SQL Server 2018
- SQL Server Management Studio (SSMS)
- SQL Server Analysis Services (SSAS)
- Visual Studio 2019 with SSDT (SQL Server Data Tools)

---

## 🚀 Setup Instructions

### 🔄 1. Database Restoration (`D1.bak`)

1. Save the `.bak` file locally (e.g. `C:/Users/Public`)
2. Open SQL Server Management Studio
3. Right-click **Databases** → **Restore Database**
4. Choose **Device** → Click "..." → Add the `.bak` file
5. Confirm settings and click **OK** to restore

---

### 📊 2. Business Intelligence Solution (`D2.sln`)

1. Open Visual Studio with SSDT installed
2. Go to **File → Open → Project/Solution**
3. Navigate to `D2` folder and open `D2.sln`
4. In **Solution Explorer**, double-click the `.cube` file
5. Deploy the solution to your local SSAS instance

---

## ✅ Prerequisites

- Microsoft SQL Server 2018
- SQL Server Management Studio
- Visual Studio with SSDT installed

---

## 🧩 Troubleshooting

### 🗃️ Database Restore Issues
- Save the `.bak` file in `C:/Users/Public` to avoid permission errors
- Ensure SQL Server service is running
- Check the database compatibility level (SQL Server 2018)

### 📉 BI Solution Issues
- Ensure SSAS is properly configured
- Verify SSDT and required components are installed
- Check Data Source connection settings in your `.dsv` file

---

## 📂 Project Components

- **D1** – Relational Database Backup (`.bak`)
- **D2** – BI Solution for SSAS (`.sln`)

---

## 🧾 Version

**1.0.0**  
📌 *This project uses real business data and is intended strictly for academic purposes.*

---

## 👨‍💻 Author

**Atharva Sapkal**  
MSc Data Science  
University of Surrey
