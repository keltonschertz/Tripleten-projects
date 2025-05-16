
# 🛒 Superstore Returns Analysis Project

## 🎯 Objective
Help the CEO of the Superstore understand why customers are returning their orders and recommend actions to reduce return volume. Your analysis will include building visualizations, constructing a dashboard, and presenting findings in a compelling, data-driven story.

---

## 🔍 Part 1: What is Causing Returns?

### 🛠️ Data Preparation
- Join the `Returns` table to the `Orders` table using a **LEFT JOIN**
- Create a calculated field `Returned`:
  - `"Yes"` = 1
  - `null` = 0
- **Return Rate** = AVG(`Returned`)
- **Total Returns** = SUM(`Returned`)

### 📊 Required Worksheets
1. **Scatterplot**: Total Sales vs. Total Returns by Product Subcategory
2. **Bar Chart**: Return Rate by Product Category
3. **Customer Return Rate**: 
   - Filter out customers with only 1 order
4. **Geographic Map**: Return Rate by State/City
5. **Time Series**: Return Rate by Month/Week
6. **Composite Charts** (2):
   - Example: Date vs. Category with Return Rate
   - Example: Region vs. Subcategory with Return Rate

---

## 🧱 Part 2: Building a Dashboard for Monitoring Returns

### 📋 Dashboard Design Requirements
- **Mockups**:
  - Create 3 pen-and-paper dashboard sketches
  - Submit photos/scans
- **Choose One**:
  - Create your dashboard in Tableau based on your favorite sketch
- **Template Setup**:
  - Use empty containers to define layout
  - Submit a screenshot of your layout
- **Finalize Dashboard**:
  - Add worksheets to the layout
  - Add titles, images, markers
  - Ensure usability with filters and clean design

---

## 🎤 Part 3: Presenting Your Analysis and Dashboard

### 🧵 Story Arc
Create a story in Tableau using **captions** and **story points** to guide your presentation.

**Include:**
1. Summary of your analysis
2. Measuring returns: rate vs. total cost vs. total number
3. Key root causes of returns
4. Overview of each dashboard component
5. How to interpret each chart
6. Demonstrate dashboard usage and filter interaction
7. Recommend actions from dashboard insights
8. Final conclusion with next steps (e.g., dashboard deployment)

### 🖼️ Tableau Story
- Add all relevant worksheets and new charts as needed
- Build Story Points and dashboards to support each section

---

## 📽️ Final Presentation

### Options:
- **Record a 3–5 minute video** of your Tableau Story:
  - **Mac**: QuickTime Player → File → New Screen Recording
  - **Windows**: `Windows Key + Alt + R`
- **OR Submit as PDF** presentation

---

## ✅ Submission Checklist
- [ ] Joined dataset with calculated return field
- [ ] Six charts visualizing return causes
- [ ] Dashboard sketches (3) and final design
- [ ] Completed Tableau Dashboard
- [ ] Tableau Story with captions
- [ ] Final presentation (Video or PDF)

---

## 🧠 Pro Tip
Use clear labels, consistent formatting, and actionable insights. Your goal is to empower the CEO with clarity, not just data.

