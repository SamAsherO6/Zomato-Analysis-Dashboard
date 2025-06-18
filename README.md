# 🍽️ Zomato Power BI Dashboard – Interactive Data Analysis & Insights

This repository contains a comprehensive Power BI project focused on analyzing and visualizing Zomato's food delivery and customer data. The project showcases dynamic dashboards, DAX-powered measures, and visual storytelling to uncover key business insights across regions, cuisines, and customer behavior.

---

## 📊 Overview

This end-to-end dashboard uses **Power BI** and **DAX** to present real-time insights from Zomato datasets. It supports:

- Interactive filtering with slicers
- Top N rankings (Top 5, Top 10, etc.)
- Year-over-year comparisons
- Regional and demographic trends
- Clean, aesthetic visualizations with gradient effects

---

## 🔧 Features

- 💡 Dynamic Top N analysis using `RANKX` and parameter slicers
- 📅 Year and Month-based analysis using `FORMAT` and `VALUE` functions
- 📈 KPI cards and visuals for Ratings, Orders, and Demographics
- 🧩 Relationship modeling across multiple data tables
- 🎨 Custom visual design with gradient fills, themes, and icons
- 📌 Editable visual interactions for focused insight delivery

---

## 📦 Data Sources

The data was sourced from:
- Google Drive [🔗](https://drive.google.com/drive/folders/1aluMi-PHu0oZXNEcdcFYC1srG05CWuLs)
- Includes restaurant data, customer ratings, order details, and more.

---

## 🧠 Key Insights

- 🔝 **Top Cuisines**: Indian, Chinese, and Fast Food dominate order volumes.
- 🌍 **Region Performance**: Tier-2 cities are emerging as high-growth areas.
- 📱 **Engagement Trends**: Mobile app usage has overtaken desktop significantly.
- ⭐ **Customer Ratings**: Majority fall between 3.5 and 4.5, with regional spikes.
- 🕑 **Order Trends**: Post-2020 surge in orders suggests strong recovery.

---

## 🚀 Getting Started

1. Download or clone this repository.
2. Open `report.pbix` using Power BI Desktop.
3. Refresh data if needed using your local or shared source.
4. Interact with slicers, explore rankings, and view insights!

---

## 🛠️ Tools Used

- Power BI Desktop  
- Power Query  
- DAX (Data Analysis Expressions)  
- Excel / CSV for data ingestion  

---

## 📌 Useful DAX Functions Used

```DAX
-- Rank by a measure
Rank_Orders = RANKX(ALL('Table'[Restaurant]), [Total Orders], , DESC)

-- Convert string year to integer
Year = VALUE('Table'[Year_Column])

-- Format date to year
Formatted_Year = FORMAT('Table'[Date], "yyyy")
