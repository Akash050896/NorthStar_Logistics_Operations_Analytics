# 🚚 NorthStar Logistics Operations Analytics Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)
![Domain](https://img.shields.io/badge/Domain-Logistics-blue)

---

# 📌 Project Overview

The **NorthStar Logistics Operations Analytics Dashboard** provides a centralized view of logistics operations across **orders, hubs, drivers, and vehicles**.

Using operational logistics data, the dashboard helps monitor **delivery performance, hub capacity utilization, driver productivity, and fleet reliability**.

The goal of this project is to transform logistics data into **actionable insights that support operational efficiency and data-driven decision making**.

---

# 📑 Table of Contents

## 📌 Project Overview
- [Project Overview](#-project-overview)
- [Project Summary](#-project-summary)

## 🎯 Business Understanding
- [Business Problem](#-business-problem)
- [Project Objectives](#-project-objectives)
- [Project Highlights](#-project-highlights)

## 🔄 Project Workflow
- [Project Workflow](#-project-workflow)
- [Dataset Information](#-dataset-information)
- [Data Model](#-data-model)

## 📊 Dashboard & Analysis
- [Dashboard Structure](#-dashboard-structure)
- [Dashboard Insights](#-dashboard-insights)
- [Dashboard Screenshots](#-dashboard-screenshots)

## 📈 Insights & Recommendations
- [Key Insights](#-key-insights)
- [Operational Recommendations](#-operational-recommendations)

## 🧾 Conclusion
- [Conclusion](#-conclusion)

## 🛠 Technical Details
- [Tools & Technologies](#-tools--technologies)
- [Dashboard Access](#-dashboard-access)
- [How to Load the Dataset](#-how-to-load-the-dataset)
- [Project Repository Structure](#-project-repository-structure)

## 👤 Author
- [Author](#-author)
---

# 📍 Project Summary

- Built an **interactive Power BI dashboard** to monitor logistics operations.  
- Analyzed delivery performance across **orders, hubs, drivers, and vehicles**.  
- Generated insights to support **capacity planning, fleet management, and delivery optimization**.

---

# 🎯 Business Problem

**NorthStar Logistics** operates a multi-hub delivery network with numerous drivers and vehicles handling high volumes of orders.

However, the company lacked a centralized analytics solution to monitor operational performance, creating several challenges:

- Limited visibility into **delivery delays**
- Difficulty identifying **underperforming hubs and drivers**
- Lack of monitoring of **fleet utilization and breakdown trends**
- Limited insight into **customer satisfaction**
- No consolidated view of **order demand trends**

To address these issues, a **Power BI analytics dashboard** was developed to track operational metrics and support data-driven decision making.

---

# 🎯 Project Objectives

- Monitor logistics performance across hubs and deliveries  
- Track **on-time delivery rate and customer satisfaction**  
- Identify **hub capacity utilization issues**  
- Analyze **driver productivity and delays**  
- Monitor **vehicle utilization and breakdown trends**  
- Support data-driven operational planning  

---

# ⭐ Project Highlights

- Built an **interactive Power BI dashboard with four analytical views**
- Integrated logistics data across **orders, hubs, drivers, and vehicles**
- Identified operational bottlenecks affecting delivery performance
- Generated insights for **capacity planning and fleet optimization**

---

# 🔄 Project Workflow

1️⃣ **Data Import**  
Imported logistics datasets including orders, hubs, drivers, and vehicles.

2️⃣ **Data Modeling**  
Implemented a **Star Schema data model** connecting fact and dimension tables.

3️⃣ **Data Analysis**  
Created calculated measures using **DAX** to evaluate logistics performance.

4️⃣ **Dashboard Development**  
Designed interactive dashboards to monitor operational metrics.

5️⃣ **Insight Generation**  
Analyzed trends to identify operational bottlenecks and improvement opportunities.

---

# 📊 Dataset Information

The project uses **four operational datasets**.

## Orders Dataset

| Column Name | Description |
|---|---|
Order ID | Unique identifier for each order |
Order Date | Date the order was placed |
Actual Delivery Date | Delivery completion date |
Driver ID | Assigned driver |
Hub Name | Processing hub |
Vehicle Type | Vehicle used for delivery |
Delivery Time Hours | Total delivery time |
Hub Processing Time Hours | Hub processing duration |
Customer Satisfaction Score | Customer feedback rating |
Order Status | Delivered / Delayed / Cancelled |
Delay Reason | Cause of delay |

---

## Drivers Dataset

| Column Name | Description |
|---|---|
Driver ID | Unique driver identifier |
Driver Name | Driver name |
Hire Date | Joining date |
Experience Years | Years of experience |
Employment Type | Full-time / Contract |
Performance Rating | Driver performance rating |

---

## Vehicles Dataset

| Column Name | Description |
|---|---|
Vehicle Code | Unique vehicle identifier |
Vehicle Model | Vehicle model |
Purchase Date | Vehicle purchase date |
Vehicle Status | Active / Maintenance / Inactive |
Breakdown | Number of breakdown incidents |
Maintenance Count | Maintenance events |

---

## Hubs Dataset

| Column Name | Description |
|---|---|
Hub ID | Unique hub identifier |
Hub Name | Hub location |
Hub Capacity | Maximum orders hub can process |

---

# 🧩 Data Model

The Power BI report uses a **Star Schema data model**.

- **Fact Table:** `Orders`  
- **Dimension Tables:** `Drivers`, `Vehicles`, and `Hubs`

This structure enables analysis across **delivery performance, workforce productivity, and fleet operations**.

---

# 🧭 Dashboard Structure

The Power BI report contains **four dashboards**:

1️⃣ Overview Dashboard  
2️⃣ Hubs Overview  
3️⃣ Drivers Overview  
4️⃣ Vehicle Overview  

---

# 📊 Dashboard Insights

## 📊 Dashboard 1 — Overview

### 🔑 Key KPIs

- **Total Orders** — Current vs Previous Month with MoM %  
- **On-Time Delivery %** — Delivery punctuality rate  
- **Customer Satisfaction (CSAT %)** — Customer feedback score  
- **Average Delivery Time (Hours)** — Delivery turnaround time  

---

### 🏭 Hub Insights

- Total Number of Hubs  
- Orders Processed vs Hub Capacity  
- Hub Performance Ranking  

**Business Impact:** Helps identify hub bottlenecks and supports capacity planning.

---

### 🧑‍✈️ Driver Insights

- Total Drivers  
- Experience vs Rating Analysis  
- Drivers with Most Delays  

**Business Impact:** Supports driver performance monitoring and training.

---

### 🚛 Vehicle Insights

- Total Vehicles  
- Active Vehicles  
- Orders by Vehicle Model  

**Business Impact:** Helps optimize fleet utilization.

---

## 🏢 Dashboard 2 — Hubs Overview

| Visualization | Chart Type | Purpose |
|---|---|---|
Total Hubs | KPI Card | Displays number of hubs |
Orders vs Capacity | Clustered Column Chart | Compares hub capacity and orders |
Hub Performance Ranking | Ranked Bar Chart | Identifies best and worst hubs |
Hub Processing Time | Matrix Table | Shows processing efficiency |

**Business Impact:** Identifies overloaded hubs and improves workload distribution.

---

## 👨‍✈️ Dashboard 3 — Drivers Overview

| Visualization | Chart Type | Purpose |
|---|---|---|
Number of Drivers | KPI Card | Displays workforce size |
Experience vs Rating | Scatter Plot | Analyzes experience vs performance |
Drivers with Most Delays | Bar Chart | Identifies drivers causing delays |
Monthly Orders Trend | Line Chart | Tracks delivery demand trends |

**Business Impact:** Supports workforce planning and performance improvement.

---

## 🚚 Dashboard 4 — Vehicle Overview

| Visualization | Chart Type | Purpose |
|---|---|---|
Total Vehicles | KPI Card | Displays fleet size |
Active Vehicles | Donut Chart | Shows active fleet percentage |
Orders by Vehicle Model | Bar Chart | Compares fleet utilization |
Vehicle Age vs Breakdown | Scatter Plot | Analyzes breakdown trends |
Breakdown by Vehicle Code | Bar Chart | Identifies unreliable vehicles |
Orders by Vehicle Type | Donut Chart | Shows delivery distribution |

**Business Impact:** Supports predictive maintenance and fleet optimization.

---

# 🖼️ Dashboard Screenshots

### 📊 Overview Dashboard

<p align="center">
<img src="Dashboard Screenshots/overview_dashboard.jpg" width="900">
</p>

---

### 🏢 Hubs Overview

<p align="center">
<img src="Dashboard Screenshots/hubs_dashboard.jpg" width="900">
</p>

---

### 👨‍✈️ Drivers Overview

<p align="center">
<img src="Dashboard Screenshots/drivers_dashboard.jpg" width="900">
</p>

---

### 🚚 Vehicle Overview

<p align="center">
<img src="Dashboard Screenshots/vehicle_dashboard.jpg" width="900">
</p>

---

# 🔎 Key Insights

- Hub capacity imbalance may contribute to **delivery delays**
- Driver experience shows a **positive relationship with performance ratings**
- A small group of drivers accounts for **higher delay frequency**
- Older vehicles demonstrate **higher breakdown risk**
- Monitoring logistics KPIs helps identify **operational bottlenecks**

---

# 💡 Operational Recommendations

**Optimize Hub Capacity Allocation**  
Redistribute orders to avoid hub overload.

**Enhance Driver Training Programs**  
Provide targeted training for drivers with higher delay rates.

**Implement Preventive Fleet Maintenance**  
Monitor vehicle age and breakdown patterns to reduce downtime.

**Improve Route Planning**  
Analyze delivery patterns to reduce delivery times.

**Monitor Customer Satisfaction**  
Track CSAT trends to improve service quality.

---

# 🧾 Conclusion

This project provides a comprehensive view of logistics operations across **orders, hubs, drivers, and vehicles** at **NorthStar Logistics**.

The analysis highlights the importance of monitoring **delivery timelines, hub efficiency, driver productivity, and fleet reliability** to improve operational efficiency.

Using these insights, logistics teams can **optimize resources, reduce delays, and enhance customer experience**.

---

# 🛠️ Tools & Technologies

### 📊 Data Visualization
- **Power BI Desktop** — Interactive dashboard development and KPI visualization


### 📐 Data Modeling
- **Star Schema Data Model** — Structured fact and dimension tables for efficient analytics
- **Relationship Modeling** — Linking orders, hubs, drivers, and vehicles datasets

### 📈 Data Analysis
- **DAX (Data Analysis Expressions)** — Calculated measures, KPIs, and performance metrics

### 🗂️ Repository Management
- **GitHub** — Project version control and repository management

---

# 📊 Dashboard Access

The interactive dashboard is available in the Power BI report file:

```
PowerBI / Logistics Dashboard.pbix
```

Open using **Power BI Desktop**.

---

# 📥 How to Load the Dataset

1. Open **Power BI Desktop**  

2. Load the **Logistics Dashboard.pbix**.

3. Interact with dashboard using slicers.

---

# 📂 Project Repository Structure

```
NorthStar_Logistics_Operations_Analytics
│
├── Dataset
│   ├── Orders.csv
│   ├── Drivers.csv
│   ├── Vehicles.csv
│   └── Hubs.csv
│
├── PowerBI
│   └── Logistics_Dashboard.pbix
│
├── Dashboard Screenshots
│   ├── overview_dashboard.jpg
│   ├── hubs_dashboard.jpg
│   ├── drivers_dashboard.jpg
│   └── vehicle_dashboard.jpg
│
└── README.md
```

---

# 👤 Author

**Akash Kindre**

Aspiring Data Analyst with hands-on experience in **Power BI, SQL, Excel & Python** specializing in **data visualization, KPI reporting, and dashboard development**. Skilled in **data cleaning, data modeling, and business performance analysis**, with a strong focus on transforming raw data into actionable insights to support data-driven decision-making.
