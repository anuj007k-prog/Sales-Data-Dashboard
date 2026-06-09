# Mobile Sales-Data-Dashboard
# Project Headline

**Mobile Sales Dashboard – Interactive Business Intelligence Solution for Sales Performance Analysis**

---

# Project Overview

The **Mobile Sales Dashboard** is an interactive Business Intelligence (BI) solution developed to monitor, analyze, and compare mobile phone sales performance across different dimensions such as time, city, mobile models, payment methods, customer ratings, and sales trends. The dashboard provides decision-makers with a centralized view of key business metrics, enabling data-driven decisions and performance tracking.

The solution consists of three analytical pages:

1. **Dashboard Overview** – Comprehensive sales performance summary.
2. **MTD (Month-to-Date) Report** – Detailed daily sales progression and trend analysis.
3. **Same Period Last Year Analysis** – Comparative performance analysis against previous year sales.

---

# Purpose of the Project

The primary objectives of this dashboard are:

* Monitor overall mobile sales performance.
* Track sales quantity and revenue generation.
* Analyze customer purchasing behavior.
* Identify top-performing products and cities.
* Compare current sales with historical performance.
* Evaluate payment method preferences.
* Support strategic business decisions through visual analytics.

---

# Technology Stack Used
 * Data Visualization & Reporting
 * Microsoft Power BI Desktop

### Data Transformation
* **Power Query Editor**
  * Data Cleaning
  * Data Transformation
  * Data Modeling

### Data Analysis

* **DAX (Data Analysis Expressions)**

  * KPI Calculations
  * MTD Calculations
  * Same Period Last Year Measures
  * Time Intelligence Functions

### Data Source

* Mobile Sales Dataset (Sales Transactions, Product Details, Customer Information)

---

# Key Performance Indicators (KPIs)

The dashboard prominently displays the following KPIs:

| KPI               | Description                           |
| ----------------- | ------------------------------------- |
| Total Sales       | Overall revenue generated             |
| Total Quantity    | Number of mobile units sold           |
| Average Price     | Average selling price per transaction |
| Transaction Count | Total transactions completed          |

### Dashboard Snapshot

* **Total Sales:** 769M
* **Total Quantity:** 19K
* **Average Price:** 40K
* **Transactions:** 4K

---

# Dashboard Features

## 1. Dynamic Filters (Slicers)

Users can interactively filter data using:

### Time Filters

* Month Selection
* Year Selection
* Quarter Selection
* Day Selection

### Product Filters

* Mobile Model
* Brand

### Transaction Filters

* Payment Method

These filters allow users to perform detailed drill-down analysis.

---

# Dashboard Pages

---

# Page 1: Sales Overview Dashboard

This page provides a complete summary of business performance.

## Charts Used

### 1. Transaction by Payment Method (Pie Chart)

Displays sales distribution across payment methods:

* UPI
* Debit Card
* Credit Card
* Cash

**Business Insight:**

* Payment modes contribute almost equally.
* Digital payments dominate customer transactions.

---

### 2. Total Quantity by Month (Line Chart)

Tracks monthly sales volume.

**Insights:**

* Peak sales observed during March and July.
* Lower performance in February and September.
* Helps identify seasonal trends.

---

### 3. Total Sales by City (Map Visualization)

Geographical representation of sales.

**Insights:**

* Identifies high-performing regions.
* Useful for regional sales strategy and expansion planning.

---

### 4. Customer Ratings by Rating Status (Horizontal Bar Chart)

Categorizes customer feedback:

* Good
* Average
* Poor

**Insights:**

* Majority of customers provide positive ratings.
* Indicates strong customer satisfaction.

---

### 5. Brand Performance Table

Displays:

* Brand Name
* Total Sales
* Transaction Count

Brands shown:

* Apple
* Samsung
* Vivo
* Xiaomi
* OnePlus

**Insights:**

* Apple leads in revenue generation.
* Helps compare brand contribution.

---

### 6. Total Sales by Mobile Model (Bar Chart)

Highlights top-selling mobile models.

Examples:

* iPhone SE
* OnePlus Nord
* Galaxy Note 20

**Insights:**

* Identifies best-performing products.
* Supports inventory planning.

---

### 7. Total Sales by Day Name (Area Chart)

Shows sales performance by weekday.

**Insights:**

* Weekend sales tend to be higher.
* Helps optimize promotional campaigns.

---

# Page 2: MTD (Month-to-Date) Report

The MTD report tracks cumulative sales performance over time.

## Chart Used

### MTD Sales Trend (Line Chart)

Displays cumulative sales progression across months and days.

### Metrics

* Month-to-Date Sales
* Daily Growth Pattern

**Insights:**

* Shows how revenue accumulates throughout the month.
* Enables monitoring against sales targets.
* Detects performance slowdowns early.

### Business Value

Management can:

* Track monthly achievement.
* Monitor daily sales momentum.
* Take corrective actions during underperformance.

---

# Page 3: Same Period Last Year Analysis

This page compares current-year sales performance against historical data.

## Charts Used

### 1. Yearly Comparison (Clustered Column Chart)

Compares:

* Current Year Sales
* Same Period Last Year Sales

**Insights:**

* Measures annual growth.
* Identifies performance gaps.

---

### 2. Quarterly Comparison (Clustered Column Chart)

Analyzes quarter-wise performance.

**Insights:**

* Highlights strongest and weakest quarters.
* Evaluates seasonal business trends.

---

### 3. Monthly Comparison (Clustered Column Chart)

Compares monthly sales across years.

**Insights:**

* Detects recurring seasonal patterns.
* Supports forecasting.

---

### 4. Comparison Table

Displays:

* Year
* Quarter
* Total Sales
* Same Period Last Year Sales

**Insights:**

* Detailed numeric validation of graphical analysis.
* Enables granular performance comparison.

---

# DAX Measures Used

The dashboard utilizes advanced DAX calculations such as:

### Total Sales

```DAX
Total Sales = SUM(Sales[SalesAmount])
```

### Total Quantity

```DAX
Total Quantity = SUM(Sales[Quantity])
```

### Average Price

```DAX
Average Price = AVERAGE(Sales[UnitPrice])
```

### Transaction Count

```DAX
Transaction Count = DISTINCTCOUNT(Sales[TransactionID])
```

### MTD Sales

```DAX
MTD Sales =
TOTALMTD(
    [Total Sales],
    DateTable[Date]
)
```

### Same Period Last Year

```DAX
Sales SPLY =
CALCULATE(
    [Total Sales],
    SAMEPERIODLASTYEAR(DateTable[Date])
)
```

---

# Business Insights Derived

### Sales Performance

* Total sales reached **769M**, indicating strong market demand.
* Sales volume exceeded **19K units sold**.

### Customer Behavior

* Digital payment methods (UPI, Debit Card, Credit Card) are widely adopted.
* Customer ratings are predominantly positive.

### Product Analysis

* Premium mobile models contribute significantly to revenue.
* Certain models consistently outperform others.

### Geographic Analysis

* Major metropolitan cities generate the highest revenue.
* Regional sales opportunities can be identified through map analysis.

### Time-Based Trends

* Specific months show stronger sales activity.
* Weekday analysis reveals optimal selling periods.

### Growth Monitoring

* MTD reporting helps track current month progress.
* Same Period Last Year analysis measures business growth and performance consistency.

---

# Dashboard Highlights

✔ Interactive and user-friendly design
✔ Multi-page analytical reporting
✔ Dynamic filtering and drill-down capability
✔ Time intelligence using DAX functions
✔ Geographical sales analysis using maps
✔ Historical sales comparison (YoY Analysis)
✔ Real-time KPI monitoring
✔ Executive-level sales performance overview
✔ Product, customer, and payment method analysis
✔ Business decision support through actionable insights

---

# Conclusion

The **Mobile Sales Dashboard** serves as a comprehensive sales analytics platform that transforms raw transaction data into meaningful business insights. Through KPI tracking, trend analysis, geographical visualization, MTD reporting, and year-over-year comparison, the dashboard empowers stakeholders to monitor performance, identify opportunities, optimize sales strategies, and make informed business decisions. It demonstrates the effective use of **Power BI, Power Query, and DAX** to create a professional, enterprise-grade Business Intelligence solution.
