# Shield Insurance Analysis

## About Company

- Shield Insurance provides affordable and customizable insurance solutions tailored to individuals across different age groups.
- The company has a presence across Mumbai, Chennai, Delhi NCR, Hyderabad, and Indore.
- Insurance products are offered through multiple sales channels, including Offline Agents, Offline Direct, Online App, and Online Website.

---

## Problem Statement

- Shield Insurance lacked a consolidated and interactive view to monitor customer growth, revenue performance, and policy trends.
- There was limited visibility into customer behavior across different age groups, cities, sales modes, and policies.
- This made it difficult for stakeholders to identify growth trends, evaluate sales channel performance, and understand demographic impacts on revenue and expected settlement.

---

## Project Objective

- Track total customers and total revenue.
- Monitor daily and month-over-month growth trends.
- Analyze revenue and customer performance across different cities.
- Evaluate sales mode performance based on customer and revenue contribution.
- Analyze policy performance and customer distribution.
- Segment customers by age group to understand revenue and customer behavior.
- Identify high-value customer segments and effective sales channels.
- Analyze age-group-wise policy preferences and expected settlement percentages.
- Enable interactive analysis through Power BI dashboards and dynamic filters.

---

## Dataset Overview

The project consists of the following data tables:

### Dimension Tables

- **dim_customer**
  - Customer Code
  - Age
  - Age Group
  - City
  - Date of Birth

- **dim_policies**
  - Policy ID
  - Base Coverage Amount
  - Base Premium Amount

- **dim_date**
  - Date
  - Month
  - Month Sort
  - Day Type

### Fact Tables

- **fact_premiums**
  - Customer Code
  - Date
  - Policy ID
  - Sales Mode
  - Final Premium Amount

- **fact_settlements**
  - Age
  - Settlement %
  - Settlement-related values

---

## Key Terms

- **Base Coverage Amount** — The maximum amount the insurance policy covers in case of a claim.
- **Premium** — The amount paid by the customer to keep the insurance policy active.
- **Claim** — A request made by the customer to receive financial coverage for a covered loss.
- **Settlement Amount** — The amount actually paid by the insurer to settle an approved claim.
- **Settlement Percentage** — The percentage of the claim amount that has been settled or paid by the insurer.

---

## Key Insights

### Overall Snapshot

- **Total Revenue:** ₹989M
- **Total Customers:** 26.8K
- **Daily Average Revenue (DRG):** ₹5.47M
- **Daily Customer Growth (DCG):** 148.29

### City-Level Insights

- **Delhi NCR:** Highest revenue ₹402M | Highest customers 11,007
- **Indore:** Lowest revenue ₹81M | Lowest customers 2,096
- **Mumbai:** Second-highest revenue ₹240M | 6,432 customers
- **31–40 Age Group:** Highest revenue ₹309M | Highest customers 10,431
- **March:** Peak month — Revenue ₹264M | Customers 7,081
- **November:** Weakest month — Revenue ₹132M | Customers 3,787

### Sales Mode Insights

- **Offline Agent:** Dominates customers
  - Customers: 14,873 (55.41%)
  - Revenue: ₹551M (55.67%)

- **Online App:**
  - Customers: 4,302 (16.00%)
  - Revenue: ₹161M (16.28%)

- **Offline Direct:**
  - Customers: 4,256 (15.9%)
  - Revenue: ₹153M (15.47%)

- **Online Website:** Lowest contribution
  - Customers: 3,410 (12.70%)
  - Revenue: ₹125M (12.64%)

- **March:** Peak month across sales modes, with Offline Agent reaching approximately 3.5K customers and ₹134M revenue.

### Age Group Insights

- **31–40:** Highest revenue ₹309.32M | Highest customers 10,431
- **41+ Age Groups:** Strong customer base of 11,400 | Revenue approximately ₹598M
- **Under 30:** Lowest revenue contribution
  - 18–24: ₹25M
  - 25–30: ₹57M
- **Settlement Percentage:** Increases with age
  - 18–24: 37.51%
  - 25–30: 45.68%
  - 31–40: 53.53%
  - 41–50: 60.79%
  - 51–65: 65.35%
  - 65+: 74.33%
- **POL2005HEL:** Highest overall revenue contribution, particularly strong among the 65+ segment.

### Policy Insights

- **POL2005HEL:** Highest revenue contribution at approximately ₹324M with 1,968 customers.
- **POL4321HEL:** Highest customer count at 4,434 but lowest revenue contribution at approximately ₹25M.
- Only four policies generate more than ₹100M in revenue:
  - POL2005HEL
  - POL1048HEL
  - POL6303HEL
  - POL9221HEL

### Policy Preference by Age Group

- **18–30 → POL4321HEL**
- **31–40 → POL3309HEL**
- **41–50 → POL5319HEL**
- **51–65 → POL9221HEL**
- **65+ → POL2005HEL**

---

## Recommendations

- **Prioritize Core Segments:** Focus on the 31–40 and 50+ age groups to support revenue, retention, and settlement performance.
- **Address Underperforming Segments:** Investigate the under-30 age groups and lower-performing cities such as Indore for growth opportunities.
- **Strengthen Digital Adoption:** Maintain the strong Offline Agent channel while improving Online Website experience and adoption.
- **Optimize Product Portfolio:** Expand the reach of POL2005HEL and evaluate policies with high customer volumes but lower revenue.
- **Replicate City Best Practices:** Study the Delhi NCR sales pattern and identify practices that could be applied to other cities.
- **Leverage Seasonal Trends:** Use the strong March performance pattern to design campaigns aimed at improving weaker months such as November.

---

## Dashboard

The Power BI solution contains three major analytical views:

1. **General View**
   - Overall revenue and customer KPIs
   - Monthly revenue and customer trends
   - City-level performance
   - Age-group performance
   - Customer segmentation

2. **Sales Mode Analysis**
   - Customer distribution by sales mode
   - Revenue contribution by sales mode
   - Monthly customer trends by sales mode
   - Monthly revenue trends by sales mode

3. **Age Group Analysis**
   - Revenue and customer distribution by age group
   - Policy preference by age group
   - Expected settlement percentage by age group
   - Revenue by age group and sales mode
   - Customer trends by age group

---

## Dashboard Screenshots

### Home Page

![Home Page](Images/Home%20Page.png)

---

### General View

![General View](Images/General%20View.png)

---

### Sales Mode Analysis

![Sales Mode Analysis](Images/Sales%20View.png)

---

### Age Group Analysis

![Age Group Analysis](Images/Age%20Group%20Analysis.png)

---

## Tools & Technologies

- **Power BI**
- **DAX**
- **Power Query**
- **Data Modeling**
- **Data Visualization**
- **Excel**
- **SQL**

---

## Project Structure

```text
Shield_Insurance_Analysis/
│
├── Images/
│   ├── Home Page.png
│   ├── General View.png
│   ├── Sales View.png
│   └── Age Group Analysis.png
│
├── Shield Insurance Analysis.pbix
│
└── README.md
