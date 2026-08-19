# Bike Buyers
> Excel Data Cleaning, Analysis & Interactive Dashboard

---

## ⚙️ Project Type Flags
> *Check what applies. This helps reviewers and collaborators understand the nature of the work at a glance. Delete this block before publishing.*

- [ ] Exploratory Data Analysis (EDA)
- [ ] SQL Analysis / Querying
- [ ] Dashboard / Data Visualization
- [ ] Data Pipeline / ETL
- [ ] Predictive Modelling / Machine Learning
- [ ] Data Cleaning / Wrangling
- [ ] End-to-End (multiple of the above)
- [ ] Other: ___________

---

## Table of Contents
1. [Project Overview](#1-project-overview)
2. [Objectives](#2-objectives)
3. [Project Scope & Tools](#3-project-scope--tools)
4. [Data Workflow](#5-data-workflow)
5. [Data Model & Schema](#6-data-model--schema)
6. [Analysis & Metrics](#8-analysis--metrics)
9. [Key Insights](#9-key-insights)
10. [Recommendations](#10-recommendations)
11. [Assumptions & Limitations](#11-assumptions--limitations)
12. [Future Enhancements](#12-future-enhancements)
13. [Deliverables](#13-deliverables)
14. [Author](#14-author)

---

## 1. Project Overview
   
**Context:**
This project was created to demonstrate a complete Excel data-analysis workflow using a bike buyers dataset. The goal was to take raw customer data, clean and organize it, explore purchasing patterns, and turn the findings into an interactive dashboard that could be used to understand different customer segments.

**Problem Statement:**
The main challenge was to understand what characteristics were associated with customers purchasing a bike. In particular, the analysis explored whether income, commute distance, age, marital status, education, gender, and region could help explain differences between customers who purchased a bike and those who did not.

**Approach:**
I followed an end-to-end Excel workflow: preserved the raw dataset, created a working copy, cleaned inconsistent values and duplicates, created age brackets, built PivotTables, and used PivotCharts and slicers to analyze and filter customer segments.

**Outcome:**
The project produced an interactive Excel dashboard containing visualizations for average income, customer commute distance, and bike purchases by age group. Interactive slicers were also added for marital status, region, and education, allowing users to explore different customer segments.


---

## 2. Objectives

- **Primary Objective:**
  Analyze customer characteristics and identify patterns associated with bike purchases.
  
- **Secondary Objective 1:**
  Clean and standardize the raw customer dataset so that it could be used reliably for analysis.
- **Secondary Objective 2:**
  Compare bike purchasers and non-purchasers across income, commute distance, gender, and age groups.
- **Secondary Objective 3:**
  Build an interactive Excel dashboard that allows users to filter and explore customer segments.

---

## 3. Project Scope & Tools

### Scope

| Dimension | Details |
|-----------|---------|
| **In Scope** | Customer demographic and bike-purchase information |
| **Out of Scope** | External datasets not included in the original file |
| **Purchase Analysis** | Customers who purchased vs. did not purchase a bike, Detailed sales revenue or profitability analysis |

Granularity
The dataset is analyzed at the individual customer/person level, with each row representing customer information and whether that person purchased a bike.

### Tools & Technologies

| Category | Tool(s) Used |
|----------|-------------|
| Data Storage | Excel workbook |
| Data Processing | Microsoft Excel |
| Analysis | Excel PivotTables, formulas, filtering and segmentation |
| Visualization | Excel PivotCharts |
| Version Control | GitHub |
| Other | Excel slicers and Find & Replace |

---


## 4. Data Workflow

1. **Source:**
   
 The project uses a bike buyers/customer dataset containing demographic, socioeconomic, lifestyle, and purchase information. The transcript indicates that the dataset was obtained through a GitHub repository.
 
2. **Ingestion:**
   
 The dataset was opened in Excel and copied into a separate Working Sheet, while the original dataset was preserved as Raw Data.

3. **Cleaning & Transformation:**
   
 The main cleaning steps included:
- Checking for and removing duplicate records.

- Converting marital-status abbreviations from M/S to Married/Single.

- Converting gender abbreviations from M/F to Male/Female.

- Standardizing income formatting as currency.

- Reviewing categorical fields for inconsistencies.

- Reviewing commute-distance categories.

- Creating age brackets to make age analysis easier to interpret.

- Renaming the corrected field back to Marital Status after an accidental replacement during the cleaning process.

4. **Analysis:**
   
PivotTables were created to analyze:
- Average income by gender and bike-purchase status.

- Customer commute distance by bike-purchase status.

- Bike purchases across age brackets.

5. **Output / Visualization / Reporting:**
   
The analysis was presented through an interactive Excel dashboard containing:
- Average income visualization.

- Customer commute-distance visualization.

- Customer age-bracket visualization.

- Marital-status slicer.

- Region slicer.

- Education slicer.

The slicers were connected to the different PivotCharts so users could filter the dashboard across multiple dimensions.


---

## 5. Data Model & Schema

### Dataset / Table: `[name]`

| Field Name | Data Type | Description | Example Value |
|------------|-----------|-------------|---------------|
| ID | int  | Unique identifier for each person | 10001 |
| Marital Status | [string  | Whether the person is married or single | Married |
| Gender | string  | Customer gender | Female |
| Income | numeric | Customer Income | $55,000 |
| Children | int | Number of Children | 2 |
| Education | string  | Customer education level | Bachelors |
| Occupation` | string  | Customer occupation category | Skilled manual |
| Homeowner | string / boolean |Whether the customer owns a home | Yes |
| Cars |  int  | Numbers of cars owned | 2 |
| Commute distance | numeric | Customer commute-distance category | 2-5 Miles |
| Region | string | Customer geographic region | Europe |
| Age | int | Customer age | 42 |
| Purchased Bike | string | Whether the customer purchased a bike | Yes |

---

## 6. Analysis & Metrics

### Analytical Approach

The analysis was primarily exploratory and descriptive. I used Excel PivotTables to group customers into meaningful segments and compare differences between customers who purchased a bike and those who did not.

Rather than trying to build a predictive model, the project focused on making the existing customer data easier to understand and turning those observations into an interactive dashboard.

### Key Metrics Defined

| Metric | Plain-Language Definition | Why It Matters |
|--------|--------------------------|----------------|
| Average Income | Average income of customers within a selected segment | Shows purchasing behavior across different customer groups |
| Bike Purchase Count | Number of customers who purchased or did not purchase a bike | [What decision or question it answers] |
| Commute Distance | Customer’s reported distance from work/commuting category | Helps identify whether commuting distance is associated with bike purchases |
| Bike Purchases by Age Bracket | Number of purchases across grouped age categories | Helps identify which age groups appear more active in the dataset |

### Methods Used

- Descriptive analysis using Excel PivotTables.
- Group comparison between bike purchasers and non-purchasers.
- Average income analysis by gender and purchase status.
- Customer segmentation by age bracket.
- Purchase comparison by commute distance.
- Interactive filtering using Excel slicers
- Visual exploration through PivotCharts.

---

## 7. Key Insights

**Insight 1: Income**
The dashboard showed differences in average income between customers who purchased bikes and those who did not. In the transcript’s example, customers who purchased bikes generally had somewhat higher average incomes than those who did not.

**Insight 2: Gender**
The analysis also showed differences between male and female customers in average income within the dataset.

**Insight 3: Age**
Grouping customers into age brackets made the purchase pattern much easier to interpret than displaying every individual age. The transcript observed that customers in the middle age group appeared to account for a large share of bike purchases.

**Insight 4: Commute Distance**
Commute distance showed different purchase patterns across the available distance categories. This was included because commuting behavior could be relevant when evaluating potential bike customers.

**Insight 5: Customer Segmentation**
The slicers demonstrated that customer behavior could change substantially when filtering by combinations such as:
Marital status
Region
Education
This makes the dashboard more useful than looking at overall averages alone.


---

## 10. Recommendations

<!--
  Action-oriented. Addressed to a real audience.
  Tied explicitly to the insight that supports each one.

  WHAT GOOD LOOKS LIKE:
  Priority: High
  Recommendation: "Conduct a fulfilment audit for home goods deliveries
                   in Region A - specifically investigating whether returns
                   correlate with a particular warehouse, carrier, or SKU batch."
  Based On: Insight 1 - return rate anomaly in Region A
  Owner: Operations / Supply Chain team

  WHAT TO AVOID:
  ❌ "Improve the return rate."
     (Not actionable. Doesn't say who, how, or where to start.)
  ❌ "Further analysis is needed."
     (This is a placeholder, not a recommendation.)
-->

| Priority | Recommendation | Based On | Suggested Owner |
|----------|---------------|----------|-----------------|
| High | [Specific, actionable step] | [Insight it comes from] | [Who should act] |
| Medium | [Specific, actionable step] | [Insight it comes from] | [Who should act] |
| Low | [Exploratory or longer-term suggestion] | [Insight it comes from] | [Who should act] |

---

## 11. Assumptions & Limitations

<!--
  WHAT GOOD LOOKS LIKE:
  Assumption: "Transaction records were assumed to be complete for all five regions.
               No validation was performed against source system record counts."
  Limitation: "The analysis cannot distinguish between returns initiated by
               the customer vs. returns initiated by the business (e.g., recalls).
               If business-initiated returns are concentrated in Region A, the
               return rate finding may reflect a policy decision, not a quality issue."

  WHAT TO AVOID:
  ❌ Leaving this section blank or writing "None known."
     Every project has limitations. Documenting them is a sign of
     analytical maturity - not a confession of failure.
-->

### Assumptions
- [What did you treat as true without being able to verify?]
- [What simplifications did you make for scope or feasibility?]
- [What domain rules or definitions did you accept as given?]

### Limitations
- [What gaps exist in the data?]
- [What analysis was out of scope but could affect interpretation?]
- [What would a more rigorous version of this project include?]
- [Are there known biases in the data source or collection method?]

> *The goal here is pre-emptive Q&A. What would a thoughtful skeptic push back on? Document the answer here, before they ask.*

---

## 12. Future Enhancements

<!--
  WHAT GOOD LOOKS LIKE:
  ✅ "Automate the monthly data pull from the POS export folder using
      a scheduled Python script, replacing the current manual process."
  ✅ "Expand the return rate analysis to include carrier-level data,
      which was unavailable in this dataset but exists in the logistics system."

  WHAT TO AVOID:
  ❌ "Add a machine learning model."
     (Vague, and disconnected from the actual findings of this project.)
  ❌ Listing aspirational features that don't follow logically from the work.
-->

- [ ] [Enhancement 1 - specific and traceable to a real gap in this project]
- [ ] [Enhancement 2]
- [ ] [Enhancement 3]
- [ ] [Enhancement 4]

---

## 13. Deliverables

| Deliverable | Description | Location |
|-------------|-------------|----------|
| [Name] | [What it contains] | [`/path/to/file`] |
| [Name] | [What it contains] | [`/path/to/file`] |
| [Name] | [What it contains] | [`/path/to/file`] |

---

## 14. Author

**[Your Name]**
[Your role or title - current or target]

- 🔗 [LinkedIn URL]
- 💼 [Portfolio or GitHub profile URL]
- 📧 [Email - optional]

---

*Last updated: [Month YYYY]*
*If this template helped you, consider starring the repository.*
