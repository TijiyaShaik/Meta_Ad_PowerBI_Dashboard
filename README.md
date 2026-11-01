# 📊 Meta Ad Performance Analysis | Power BI

## 📌 Project Overview

The **Meta Ad Performance Analysis** project consists of two interactive Power BI dashboards developed to analyze advertising performance across Facebook and Instagram.

Both dashboards utilize the same underlying dataset, business requirements, KPIs, and data model. However, the analysis is presented separately for each platform to understand its individual advertising performance.

The project focuses on evaluating advertisement reach, user engagement, audience demographics, geographical distribution, conversion performance, and campaign effectiveness.

The primary objective is to transform raw advertising data into meaningful business insights that help marketing teams evaluate campaign performance, optimize advertising strategies, and make data-driven decisions.

---

## 🎯 Business Objectives

* Analyze the advertising performance of Facebook and Instagram separately.
* Measure advertisement reach, clicks, engagement, and purchases.
* Identify the most effective advertisement formats.
* Understand audience engagement based on gender, age, and geographical location.
* Analyze weekly, monthly, and hourly engagement patterns.
* Evaluate campaign budgets and advertising performance.
* Identify conversion funnel gaps and opportunities to improve purchase rates.

---

## 🛠️ Tools & Technologies

| Technology            | Purpose                                   |
| --------------------- | ----------------------------------------- |
| Microsoft Power BI    | Dashboard development and visualization   |
| Power Query           | Data cleaning and transformation          |
| DAX                   | Calculated measures and KPI development   |
| Microsoft Excel / CSV | Dataset storage and preparation           |
| Data Modeling         | Establishing relationships between tables |

---

# 📊 Project Dashboards

This project contains two separate dashboards developed using a common dataset.

## 1. Facebook Ad Performance Dashboard

Analyzes Facebook advertising performance through interactive visualizations and KPI metrics.

**Dashboard Preview**

<!-- Add your Facebook dashboard screenshot below -->

<img width="1920" height="1020" alt="Screenshot 2026-11-01 105032" src="https://github.com/user-attachments/assets/8d575793-0ebe-4462-974a-533759e3a4ce" />


**Key Analysis:**

* Overall advertising performance and KPI metrics.
* Gender-wise and age-group engagement analysis.
* Country-wise advertising performance.
* Weekly and hourly engagement trends.
* Calendar-based engagement analysis.
* Advertisement type performance.


---

## 2. Instagram Ad Performance Dashboard

Analyzes Instagram advertising performance independently to understand audience behavior and campaign effectiveness.

**Dashboard Preview**

<!-- Add your Instagram dashboard screenshot below -->

<img width="1920" height="1020" alt="Screenshot 2026-11-01 105056" src="https://github.com/user-attachments/assets/08054be6-fac3-47bf-8101-923737fef733" />


**Key Analysis:**

* Overall advertising performance and KPI metrics.
* Gender-wise and age-group engagement analysis.
* Country-wise advertising performance.
* Weekly and hourly engagement trends.
* Calendar-based engagement analysis.
* Advertisement type performance.


---

## 📂 Dataset Description

The project uses four interconnected tables representing Meta advertising activities.

| Table Name  | Description                                                                                                   |
| ----------- | ------------------------------------------------------------------------------------------------------------- |
| `ad_events` | Stores advertisement interaction events such as impressions, clicks, shares, comments, and purchases.         |
| `ads`       | Contains advertisement details, including platform, ad type, campaign association, and targeting information. |
| `campaigns` | Contains campaign information such as campaign name, start date, end date, duration, and allocated budget.    |
| `users`     | Contains audience demographic information such as gender, age, age group, country, location, and interests.   |

### Data Model

The project follows a **Star Schema** data modeling approach.

* **Fact Table:** `ad_events`
* **Dimension Tables:** `ads`, `campaigns`, `users`

### Table Relationships

* `ad_events` → `ads` using `ad_id`
* `ads` → `campaigns` using `campaign_id`
* `ad_events` → `users` using `user_id`

These relationships enable analysis across advertising events, campaigns, advertisement formats, and audience demographics.

---

## 📈 Key Performance Indicators (KPIs)

The dashboards track the following business metrics:

| KPI                         | Description                                                 |
| --------------------------- | ----------------------------------------------------------- |
| Impressions                 | Total number of times advertisements were displayed.        |
| Clicks                      | Total number of clicks received by advertisements.          |
| Shares                      | Total number of times advertisements were shared.           |
| Comments                    | Total number of comments received.                          |
| Purchases                   | Total number of purchases generated through advertisements. |
| Engagements                 | Total interactions, including clicks, shares, and comments. |
| CTR                         | Percentage of impressions that resulted in clicks.          |
| Engagement Rate             | Percentage of impressions that resulted in engagements.     |
| Conversion Rate             | Percentage of clicks that resulted in purchases.            |
| Purchase Rate               | Percentage of impressions that resulted in purchases.       |
| Total Budget                | Total budget allocated across campaigns.                    |
| Average Budget per Campaign | Average budget allocated to each campaign.                  |

### KPI Formulas

| Metric          | Formula                           |
| --------------- | --------------------------------- |
| CTR             | (Clicks / Impressions) × 100      |
| Engagement Rate | (Engagements / Impressions) × 100 |
| Conversion Rate | (Purchases / Clicks) × 100        |
| Purchase Rate   | (Purchases / Impressions) × 100   |
| Average Budget  | Total Budget / Campaign Count     |

---

## 📊 Dashboard Visualizations

Both dashboards include the following visualizations:

| Visualization             | Chart Type           | Purpose                                                                   |
| ------------------------- | -------------------- | ------------------------------------------------------------------------- |
| Target Gender Analysis    | Donut Chart          | Analyze performance across gender segments.                               |
| Target Age Group Analysis | Bar Chart            | Identify the most responsive age groups.                                  |
| Geographic Distribution   | Map                  | Understand country-wise advertising performance.                          |
| Calendar Month Analysis   | Calendar Heat Map    | Identify daily and monthly activity patterns.                             |
| Weekly Engagement Trend   | Stacked Column Chart | Compare weekly performance across ad types.                               |
| Hourly Engagement Trend   | Area Chart           | Identify peak engagement hours.                                           |
| Ad Type Performance       | Matrix               | Compare performance across different advertisement formats and platforms. |

**Interactive Features:**

* Dynamic metric selection.
* Platform-specific filtering.
* Interactive charts and visualizations.
* KPI-based performance analysis.

---

## 🔍 Key Business Insights

Based on the analyzed dataset, the following overall insights were identified:

### Overall Performance

| Metric                      |  Value |
| --------------------------- | -----: |
| Impressions                 |   216K |
| Clicks                      |  25.4K |
| Shares                      |   1.3K |
| Comments                    |   2.6K |
| Purchases                   |   1.3K |
| Engagements                 |    29K |
| CTR                         | 11.76% |
| Engagement Rate             | 13.56% |
| Conversion Rate             |  5.21% |
| Purchase Rate               |  0.61% |
| Total Budget                |   2.5M |
| Average Budget per Campaign |  50.7K |

*Note: These are overall dataset figures, not individual Facebook or Instagram figures.*

### Audience Insights

* Female audiences contributed the largest share of engagement.
* The 20–30 age group showed the highest engagement.
* The United States, India, Brazil, Germany, and the United Kingdom were among the major contributing countries.

### Time-Based Insights

* Engagement remained relatively consistent across weeks.
* Afternoon and evening hours showed higher engagement.
* Early morning hours recorded comparatively lower engagement.
* Certain dates showed increased advertising activity.

### Advertisement Type Insights

* Video advertisements demonstrated strong CTR and engagement performance.
* Stories advertisements generated higher impressions and competitive conversion performance.
* Carousel and Image advertisements also contributed to overall engagement.

---

## 💡 Business Recommendations

Based on the dashboard findings, the following recommendations can help improve advertising performance:

1. **Improve Conversion Efficiency:** Optimize landing pages and simplify the purchase process to reduce customer drop-offs.

2. **Audience Optimization:** Focus on highly engaged audience segments while validating their actual purchase behavior.

3. **Advertisement Format Optimization:** Allocate more budget to high-performing Video and Stories advertisements based on conversion and cost efficiency.

4. **Geographical Optimization:** Focus on high-performing countries and evaluate conversion performance before increasing regional budgets.

5. **Ad Scheduling:** Prioritize afternoon and evening advertising slots based on observed engagement patterns.

6. **Retargeting Campaigns:** Target users who clicked or interacted with advertisements but did not complete purchases.

7. **Budget Optimization:** Evaluate campaign-level spending against actual purchases and revenue before reallocating budgets.

---

## 📁 Repository Structure

```text
Meta_Ad_PowerBI_Dashboard/
│
├── README.md
│
├── Dashboards/
│   │
│   ├── Facebook/
│   │   └── Facebook_dashboard.png
│   │
│   └── Instagram/
│       └── Instagram_dashboard.png
│
├── Dataset/
│   ├── ad_events.csv
│   ├── ads.csv
│   ├── campaigns.csv
│   └── users.csv
│
├── Documentation/
│   ├── Business_Requirements.md
│   └── Domain_Knowledge.md
│
└── meta ad dashboard.pbix

```

---

## 🚀 How to Use This Project

1. Clone or download this repository.
2. Install Microsoft Power BI Desktop.
3. Navigate to the `Dashboards` folder.
4. Open either the Facebook or Instagram `.pbix` file.
5. If necessary, update the dataset file paths in Power Query.
6. Refresh the data.
7. Explore the interactive dashboards and visualizations.

---

## 📌 Conclusion

The Meta Ad Performance Analysis project provides a comprehensive view of Facebook and Instagram advertising effectiveness through two separate Power BI dashboards.

By combining audience analysis, engagement tracking, conversion metrics, and campaign performance analysis, the project identifies opportunities to improve advertising efficiency and optimize marketing strategies.

This project demonstrates practical knowledge of **Power BI, DAX, Power Query, data modeling, data visualization, and business intelligence**, transforming raw advertising data into actionable business insights.

---

**Project Category:** Data Analytics | Business Intelligence

**Developed Using:** Microsoft Power BI

**Author:** Tijiya Bhanu
