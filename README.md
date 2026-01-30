# cyclistic-bike-share-analysis
Data analysis of Cyclistic bike-share usage to identify behavioral differences between casual riders and annual members.
# Cyclistic Bike-Share Analysis  
**Capstone Project – Google Data Analytics Professional Certificate**

## 📌 Business Objective
The purpose of this analysis is to understand how **annual members** and **casual riders** use Cyclistic bikes differently and to identify **data-driven marketing strategies** that can convert casual riders into annual members.

---

## 📊 Data Sources
This project uses **historical Cyclistic (Divvy) bike-share trip data** provided as part of the Google Data Analytics Capstone Project.

- **Timeframe:** Q1 2019 and Q1 2020  
- **Format:** CSV files  
- **Key fields:** Ride timestamps, station data, ride duration, bike type (where available), and rider classification  
- **Privacy:** All data is anonymized and contains no personally identifiable information  

---

## 🧹 Data Cleaning & Preparation
The datasets were cleaned and standardized using **R**.

Key steps included:
- Standardizing schemas across datasets from different years
- Converting ride duration to minutes for consistent measurement
- Mapping rider classifications to a common format (`member`, `casual`)
- Removing records with missing timestamps or invalid durations
- Trimming extreme outliers above the **99th percentile** to prevent skewed averages
- Creating derived features (day of week, hour of day, month)

This resulted in a clean, analysis-ready dataset representing typical rider behavior.

---

## 🔍 Analysis Summary
The analysis revealed clear behavioral differences between rider types:

- **Annual members**
  - Account for **91.7% of total rides**
  - Take short, consistent trips (median ≈ **8.4 minutes**)
  - Usage patterns align with **commute and routine travel**

- **Casual riders**
  - Account for **8.3% of total rides**
  - Take significantly longer trips (median ≈ **20.0 minutes**)
  - Usage patterns indicate **leisure-oriented behavior**

These differences highlight strong opportunities for targeted conversion strategies.

---

## 📈 Key Visualizations

## 📊 Power BI Dashboard

The final visual analysis was built in **Power BI** using summary-level data exported from R.  
This dashboard highlights key behavioral differences between casual riders and annual members to support data-driven marketing decisions.

![Power BI Dashboard](powerbi_cyclistic_dashboard.png)


The analysis includes visualizations covering:
- Total rides by rider type
- Average ride duration (trimmed)
- Ride frequency by day of week
- Ride frequency by hour of day
- Monthly ride trends
- Ride duration distribution (boxplot)

Visuals are saved in the `/visuals` folder.

---

## 💡 Recommendations
1. **Ride-Based Membership Incentives**  
   Offer ride credits from long casual trips toward annual membership upgrades to position membership as a cost-saving option.

2. **Behavior-Triggered Upgrade Campaigns**  
   Target casual riders with frequent short rides using trial or discounted membership offers.

3. **Seasonal Membership Promotions**  
   Launch time-limited promotions during peak leisure usage periods to capture high-intent casual riders.

---

## 🛠 Tools Used
- **R** (tidyverse, lubridate, ggplot2)
- RStudio
- GitHub

---

## 📁 Repository Structure
