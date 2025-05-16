
# 📦 E-Commerce Analytics Project

## 🎯 Objective
Welcome to your first project as a Junior Analyst! You've been hired by an e-commerce company to analyze raw transaction logs and uncover valuable insights through a structured, multi-part analysis.

---

## 📁 Dataset Description
You’ll work with data from the **`raw_user_activity`** sheet, where each row logs a customer interaction on the website:

- **user_id**: Unique customer ID
- **event_type**: Type of user activity (view, cart, purchase)
- **category_code**: Product category
- **brand**: Brand of the product
- **price**: Product price in USD
- **event_date**: Date of the event (YYYY-MM-DD)

---

## 🧩 Part 1: Conversion Funnel

### Goal
Measure how effectively product views turn into purchases.

### Steps
- Create a new sheet: **`conversion_funnel`**
- Use a **pivot table** to count **unique users** at 3 funnel stages:
  1. Product Views
  2. Cart Opened
  3. Purchase
- Add:
  - **Total Conversion Rate**
  - **Step-by-Step Conversion Rate**

---

## 📊 Part 2: Prepare for Cohort Analysis

### Filter for Purchases
- Create a new sheet: **`purchase_activity`**
- Filter `raw_user_activity` to **purchases only**
- Copy and paste into `purchase_activity` (should have 4,845 rows incl. header)

### First Purchase Dates
- Insert pivot table in new sheet: **`first_purchase`**
- Show the **earliest event_date** for each user
- Use `VLOOKUP()` in `purchase_activity` to assign **first_purchase_date**

### Monthly Grouping
In `purchase_activity`, add:
- **event_month** (Column H): `TEXT(event_date, "YYYY-MM")`
- **first_purchase_month** (Column I): `TEXT(first_purchase_date, "YYYY-MM")`
- **cohort_age** (Column J): `DATEDIF(first_purchase_date, event_date, "M")`

---

## 📈 Part 3: Retention Rates

### Group into Cohorts
- New pivot table in sheet: **`cohort_analysis`**
- Rows = `first_purchase_month`
- Columns = `cohort_age`
- Values = count of unique users

### Calculate Retention Rates
- New sheet: **`retention_rates`**
- Rows: each cohort (A3:A7)
- Columns: cohort ages 1 to 4 (B2:E2)
- Formula in B3: `% Retained = Age_N / Age_0` (use fixed reference)

---

## 🧹 Part 4: Final Touches

### Executive Summary
Fill in the **`Executive Summary`** sheet with:
- Results from `conversion_funnel` and `retention_rates`
- Description of raw data, assumptions, and methods used

### Organize Tabs
Reorder your spreadsheet tabs:
1. Table of Contents
2. Executive Summary
3. Analytical Result Sheets
4. Calculation Sheets
5. Raw Data

### Formatting
- Format dates and numbers
- Add borders, bold headers
- Freeze rows
- Highlight calculated cells

---

## ✅ Deliverables
- Clean, professional spreadsheet
- Conversion funnel
- Retention rate analysis
- Executive-ready documentation and formatting

---

## 🧠 Tips
Put yourself in the executive’s shoes—clarity, readability, and insight are key!

