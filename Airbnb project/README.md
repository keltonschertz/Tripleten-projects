
# 📊 Manhattan Airbnb Market Analysis

## Overview
This project provides data-driven insights into the Manhattan vacation rental market using Airbnb data. The goal is to guide investment decisions by identifying the most attractive neighborhoods and property types for vacation rentals, and estimating their revenue potential.

---

## 📌 Objectives
We aim to answer two main business questions:

### 1. Which neighborhoods and property sizes are most attractive for vacation rentals?
- Identify the top 10 neighborhoods in Manhattan based on recent guest activity.
- Analyze property sizes (i.e., number of bedrooms) to determine what is most popular.
- Discover if neighborhood preferences vary when it comes to property size.

### 2. How much money did these listings generate?
- Estimate annual revenue for the most attractive listings using calendar and pricing data.
- Rank the top-performing listings by revenue.

---

## 📂 Data Sources
- **Listings**: Contains details for each property, including neighborhood, bedroom count, and total reviews.
- **Calendar**: Contains daily availability and pricing for each listing.

---

## 🧹 Data Cleaning & Preparation

### Neighborhood Name Standardization
- The `neighborhood` column is cleaned to fix capitalization and remove trailing spaces.
- Cleaned values are stored in a new column: `neighborhood_clean`.

### Filtering Listings
- Only listings with reviews in the last 12 months are used (`number_of_reviews_ltm`).
- A pivot table is created to identify the **top 10 neighborhoods** based on recent activity.

---

## 🏡 Property Size Analysis
- Listings are grouped by neighborhood and bedroom count.
- The most attractive property size is identified for each top neighborhood.
  - In most cases: **1-bedroom**
  - Exception: **Midtown** prefers **studio apartments**

---

## 🧮 Revenue Calculation

### Calendar Data
- A new column `revenue_earned` is added:
  - If `available` = `"f"` → `revenue_earned = adjusted_price`
  - If `available` = `"t"` → `revenue_earned = $0`

### Listings Data
- Another `revenue_earned` column is created using a **SUMIF** formula:
  - Total 30-day revenue for each listing is pulled from the calendar.
  - **Estimated Annual Revenue = 30-day total × 12**

### Top Listings Filter
- A new binary column `top_listing` is created:
  - Value = 1 if the listing is in a top neighborhood **and** matches the most attractive bedroom size for that neighborhood.
  - Else, value = 0

---

## 📈 Final Output
- A pivot table is created using:
  - Filter: `top_listing = 1`
  - Values: `revenue_earned`
  - Sorted to display top listings by estimated annual revenue.

---

## 🛠 Tools Used
- Microsoft Excel / Google Sheets
  - Pivot Tables
  - Data Cleaning (Formulas, Text Functions)
  - Conditional Columns (`IF()`, `SUMIF()`)

---

## 📌 Recommendations
Based on this analysis, investors should focus on:
- **Top-performing neighborhoods** with high guest engagement
- **1-bedroom apartments** (or studios in Midtown) to align with demand
- **Listings with high adjusted_price and occupancy**, as they yield the most revenue

---

## 📧 Contact
For questions or further insights, please reach out to the data team at: `yourname@yourdomain.com`
