# Music Institute Sales Dashboard

## 📊 Project Overview
This repository contains a professional, executive-ready **Sales Dashboard** built natively within Microsoft Excel. The project moves away from traditional, fragile cell-based formulas and instead implements a robust Business Intelligence pipeline (**ETL ➡️ Data Modeling ➡️ Analytics**) directly inside Excel. 

The dashboard provides deep insights into revenue generation, customer demographics, and regional performance for a global music education platform.

---

## 🛠️ Tech Stack & Architecture
Rather than relying on manual data manipulation, this project leverages Excel's modern data engine to ensure scalability and one-click refresh automation:

* **Power Query:** Used for the Extract, Transform, and Load (ETL) process. Cleaned raw transactional data, handled data type modifications, and built a custom **Date Dimension (Calendar Table)** to facilitate smooth time-intelligence tracking.
* **Power Pivot (Data Model):** Established a star-schema-like data model by connecting the transactional sales table to the Calendar lookup table.
* **DAX (Data Analysis Expressions):** Formulated custom calculations and explicit measures to optimize reporting speed and handle complex aggregations dynamically.

---

## 📈 Key Metrics & KPIs Tracked
The dashboard surfaces critical business performance indicators across multiple operational dimensions:

* **Financial Health:** Tracks *Total Sales* (₹3,853,977) alongside *Average Order Value (AOV)* (₹15,667) to monitor revenue quality.
* **Volume Metrics:** Monitors *Total Orders* (246) and *Total Customers* (233) to gauge customer acquisition.
* **Geographical Distribution:** A line chart comparing domestic versus international performance (*India* emerging as the leading regional hub, followed by the *USA*).
* **Demographic Segmentation:** A column chart breaking down sales by age buckets, highlighting the *40+ age group* and *6-12 age group* as primary revenue-generating cohorts.
* **Product Performance:** Evaluates student interest across musical genres, showing *Carnatic Classical* leading ahead of Hindustani Classical and Hindi Film Music.

---

## 💡 Key Learnings & Methodology
1. **Separation of Layers:** Maintained clean architecture by separating the data storage/cleaning layer (Power Query) from the calculation layer (Power Pivot/DAX) and presentation layer (Pivot Charts & Slicers).
2. **Dynamic Spilling & Slicing:** Connected advanced timeline and category slicers (Year, Month) to allow stakeholders to drill down into specific date blocks seamlessly without breaking data integrity.
3. **Automated Maintenance:** Designed the backend data pipeline so that appending new raw rows to the source file requires only a single click on the "Refresh All" button to update the entire dashboard.

---

## 📁 How to Use This Repository
1. Clone the repository to your local machine.
2. Open the `.xlsx` file using Microsoft Excel (Excel 2021 or Microsoft 365 recommended for full Power Pivot compatibility).
3. Interact with the slicers on the left panel to filter the sales data by Year (2023–2024) and Month.

---
*Disclaimer: All dataset metrics and customer records used in this project are simulated for operational analysis and business intelligence portfolio demonstration purposes.*
