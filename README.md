# ✈️ Airline Performance Analytics Dashboard | Power BI

An interactive **6-page Power BI analytics application** built to analyze airline operations, revenue, customer loyalty, fleet performance, maintenance, and customer satisfaction across a **3-year period (2023–2025)**.

The project focuses on building a realistic multi-table Business Intelligence model using Power Query, DAX, relational data modeling, and interactive Power BI report design.

> **Data Note:** This is a portfolio project based on synthetic airline data created for analytics and demonstration purposes. The figures do not represent a real airline.

---

## 📊 Dashboard Overview

The report contains six interconnected analytical pages:

### 1. Executive Overview

Provides a high-level view of airline performance through:

- On-Time Performance
- Cancellation Rate
- Total Revenue
- Ticket Revenue
- Active Customers
- Revenue trends
- Revenue by fare class
- Flight distribution by geography

### 2. Flight Operations

Analyzes operational efficiency and disruption patterns:

- On-Time Performance
- Cancellation Rate
- Average Arrival Delay
- Diversion Rate
- Completed Flights
- Cancellation reasons
- Delay reasons
- Airport-to-airport performance

### 3. Revenue

Analyzes revenue generation and pricing performance:

- Total Revenue
- Ticket Revenue
- Ancillary Revenue
- Bag Fee Revenue
- Revenue per Available Seat Mile (RASM)
- Revenue growth
- Revenue by booking channel
- Revenue by fare class
- Average ticket price by route

### 4. Customer & Loyalty

Analyzes customer activity and loyalty behavior:

- Total Customers
- Active Customers
- Repeat Customer Rate
- Average Tickets per Customer
- Loyalty Points Issued
- Customer spending
- Customer segments
- Top customers by spend

### 5. Fleet & Maintenance

Evaluates aircraft efficiency, maintenance cost and fleet risk:

- Maintenance Events
- Downtime Hours
- Total Maintenance Cost
- Maintenance Cost per Event
- Flights per Aircraft
- Maintenance Cost per Aircraft
- Maintenance cost by aircraft model
- Downtime by maintenance type
- Fleet age vs. maintenance cost

### 6. Customer Satisfaction

Analyzes customer experience and NPS:

- NPS Score
- Average Customer Satisfaction
- Would Recommend %
- Promoters %
- Passives %
- Detractors %
- Satisfaction trends
- NPS by loyalty tier
- Satisfaction by complaint category

---

## 🗂️ Data Model

The project uses a **multi-table relational model** with separate fact and dimension tables.

### Dimension Tables

- `Dim_Aircraft`
- `Dim_Airport`
- `Dim_BookingChannel`
- `Dim_CancellationReason`
- `Dim_Customer`
- `Dim_Date`
- `Dim_DelayReason`
- `Dim_Employee`
- `Dim_FareClass`
- `Dim_Route`

### Fact Tables

- `Fact_Flights`
- `Fact_Bookings`
- `Fact_CustomerSatisfaction`
- `Fact_Maintenance`

The model separates transactional and descriptive data to support efficient filtering and aggregation across report pages.

A dedicated measure layer is used to organize DAX calculations and keep the model easier to maintain.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Dashboard development and data visualization |
| **Power Query** | Data import, cleaning and transformation |
| **DAX** | KPI development and analytical calculations |
| **Data Modeling** | Fact/dimension relationships and analytical model design |
| **CSV** | Source data |

---

## 📐 Key DAX Measures

The report contains approximately **50 custom DAX measures** covering multiple analytical domains.

### Operations

- Completed Flights
- Cancellation Rate %
- On-Time Performance %
- Average Arrival Delay
- Diversion %

### Revenue

- Total Revenue
- Total Ticket Revenue
- Total Ancillary Revenue
- Total Bag Fee Revenue
- Revenue per ASM (RASM)
- Revenue YoY %

### Customer & Loyalty

- Total Customers
- Active Customers
- Repeat Customer Rate
- Total Loyalty Points Issued
- Average Tickets per Customer

### Fleet & Maintenance

- Total Maintenance Cost
- Maintenance Cost per Aircraft
- Total Downtime Hours
- Flights per Aircraft
- Fleet Age

### Customer Satisfaction

- NPS Score
- Promoters %
- Passives %
- Detractors %
- Average Customer Satisfaction
- Would Recommend %

---

## 📈 Key Dashboard Metrics

The completed dashboard surfaces metrics such as:

- **75K completed flights**
- **$2.92B total revenue**
- **$2.69B ticket revenue**
- **25K customers**
- **70.1% on-time performance**
- **2.9% cancellation rate**
- **258K downtime hours**
- **$486.5M maintenance cost**
- **20.16 NPS score**

These metrics can be dynamically filtered by year, fare class, location, route, hub type, customer segment, and other dimensions.

---

## 🎯 Business Questions Answered

The dashboard is designed to answer questions such as:

- How is airline operational performance changing over time?
- Which airports and routes experience the highest disruption?
- What are the major causes of delays and cancellations?
- Which fare classes and booking channels generate the most revenue?
- Which routes have the highest ticket prices?
- Which customer segments contribute the most revenue?
- Which aircraft models have the highest maintenance costs?
- How does fleet age relate to downtime and maintenance cost?
- What factors are associated with customer satisfaction and NPS?

---

## 🎨 Dashboard Features

- Multi-page report navigation
- Page-level and cross-page slicers
- Interactive filtering
- KPI cards
- Time-series analysis
- Geographic visualization
- Matrix and tabular analysis
- Drill-style analytical exploration
- Consistent report theme and layout

---

## 📂 Repository Structure

```text
PowerBI_Airline_Analysis/
│
├── Dim_Aircraft.csv
├── Dim_Airport.csv
├── Dim_BookingChannel.csv
├── Dim_CancellationReason.csv
├── Dim_Customer.csv
├── Dim_Date.csv
├── Dim_DelayReason.csv
├── Dim_Employee.csv
├── Dim_FareClass.csv
├── Dim_Route.csv
│
├── Fact_Bookings.csv
├── Fact_CustomerSatisfaction.csv
├── Fact_Flights.csv
├── Fact_Maintenance.csv
│
├── airtravel.pbix
└── README.md
