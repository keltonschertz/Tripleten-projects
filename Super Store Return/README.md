# 📊 Superstore Profitability Analysis

## Overview

You’ve been hired as a consultant to help the Superstore evaluate its business operations and avoid bankruptcy. This project involves a multi-part analysis including profitability review, advertising strategy, and return rate diagnostics. Each question is addressed with a dedicated visualization and insights to support your recommendations.

---

## 📁 Project Structure

```
.
├── data/                      # Superstore dataset and Returns table
├── visualizations/           # All generated charts and dashboards
├── notebooks/                # Jupyter/Power BI/Tableau analysis files
├── README.md                 # This file
└── report.pdf                # Final business recommendation report
```

---

## 🧩 Part 1: Profits & Losses

### Objective:
Identify the most and least profitable segments and make product-level recommendations.

### Questions:
1. **Profit Centers & Loss-Makers:**  
   Identify the two most profitable and two least profitable *combinations of dimensions* (e.g., subcategory + region, shipping mode + product ID).  
   **Deliverable:** Matrix-style heatmaps or ranked bar charts.

2. **Product Elimination Candidates:**  
   Determine which specific products consistently lose money.  
   **Deliverable:** Filtered list of low-profit or high-loss products.

3. **Subcategory Focus Areas:**  
   Identify 3 subcategories to expand and 3 to eliminate based on profitability trends.  
   **Deliverable:** Dual bar chart with profit metrics by subcategory.

---

## 📣 Part 2: Advertising Strategy

### Objective:
Evaluate where and when advertising could boost profits effectively.

### Questions:
1. **Advertising Opportunities:**  
   Identify the 3 best state-month combinations for advertising, based on average profit per unit sold.  
   **Deliverable:** Line charts showing average monthly profit trends for each selected state.  
   **Include:** An estimate of how much could be spent on advertising in these regions.

---

## 🔁 Part 3: Returned Items

### Objective:
Assess how product returns impact profitability and identify patterns of concern.

### Questions:
1. **Returned Field Transformation:**  
   Convert the “Returned” column: `Yes = 1`, `Null = 0`.  
   **Deliverable:** Data transformation or calculated field in BI tool.

2. **High Return Rates:**  
   Analyze which products and customers have the highest return rates.  
   **Deliverables:** Two visualizations – one by product, one by customer.

3. **Profit vs Return Rate Analysis:**  
   Compare average profit against return rate by a chosen dimension (e.g., state, product type, shipping mode).  
   **Deliverable:** Scatter plot or bubble chart with interpretive analysis.  
   **Insight:** Recommend continuing or halting business based on correlation.

---

## 📌 Tools & Technologies

- Python (Pandas, Matplotlib/Seaborn/Plotly) or Tableau/Power BI for dashboards
- Excel/CSV files for source data
- Jupyter Notebook or BI dashboards for analysis
- PDF or slide deck for executive presentation

---

## ✅ Deliverables

- Individual visualizations for each question
- Accompanying insights and justifications
- Business recommendation report (PDF or PPT)

---

## 🧠 Recommendations

Use storytelling in your visualizations to clearly explain *why* a product, subcategory, or market deserves action. Be concise and impactful in presenting insights — your goal is to help decision-makers act quickly and confidently.
