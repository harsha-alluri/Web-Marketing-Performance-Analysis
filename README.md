# Web Marketing Performance Analysis

## Project Overview

This project analyzes web marketing performance data to understand website traffic, user engagement, acquisition channels, device behavior, geographic performance, and content performance.

The analysis was performed using **Power BI, Power Query, DAX, and Excel**.

The objective is to transform raw web analytics data into an interactive dashboard that helps identify traffic patterns, engagement levels, and opportunities for business improvement.

---

## Business Questions

This project addresses the following questions:

* How is website traffic changing over time?
* Which acquisition channels generate the most sessions?
* What is the website's bounce rate and exit rate?
* How many pages are viewed per session?
* Which devices generate the most traffic?
* Which countries contribute the most sessions?
* Which pages receive the highest number of pageviews?
* How does user engagement vary across channels and devices?
* Are high-traffic channels also generating good engagement?

---

## Dataset

The dataset contains web marketing and website performance information including:

* Date
* Country
* Device Category
* Channel Grouping
* Page Title
* Sessions
* Pageviews
* Unique Pageviews
* Bounces
* Exits
* Time on Page
* Page Load Time
* Other web analytics attributes

The dataset covers the period from **April 2018 to October 2018**.

---

## Data Preparation

The data was prepared using Power Query and Power BI.

Key data preparation activities included:

* Data type validation
* Missing-value inspection
* Duplicate-record analysis
* Column validation
* Data transformation
* Creation of analytical measures
* Time-based analysis
* KPI preparation

---

## Key DAX Measures

### Bounce Rate

```DAX
Bounce Rate =
DIVIDE(
    SUM('Web Marketing_Migrated Data'[Bounces]),
    SUM('Web Marketing_Migrated Data'[Sessions])
)
```

### Exit Rate

```DAX
Exit Rate =
DIVIDE(
    SUM('Web Marketing_Migrated Data'[Exits]),
    SUM('Web Marketing_Migrated Data'[Pageviews])
)
```

### Pages per Session

```DAX
Pages per Session =
DIVIDE(
    SUM('Web Marketing_Migrated Data'[Pageviews]),
    SUM('Web Marketing_Migrated Data'[Sessions])
)
```

### Average Time on Page

The dashboard also includes an average time-on-page calculation with a display measure that converts the value into a readable format such as:

`1m 38s`

---

## Dashboard

The Power BI dashboard includes:

### Executive Overview

* Total Sessions
* Total Pageviews
* Bounce Rate
* Exit Rate
* Pages per Session
* Average Time on Page

### Traffic Analysis

* Monthly Sessions
* Monthly Bounce Rate
* Sessions by acquisition channel
* Country-level traffic analysis

### User Engagement

* Bounce Rate
* Exit Rate
* Pages per Session
* Average Time on Page
* Device-level performance

### Content Analysis

* Top pages by pageviews
* Top countries
* Page performance

---

## Dashboard Preview

![Dashboard Overview](Screenshots/Dashboard_Overview.png)

---

## Tools & Technologies

* **Power BI**
* **DAX**
* **Power Query**
* **Microsoft Excel**
* **Data Cleaning**
* **Data Analysis**
* **Data Visualization**

---

## Skills Demonstrated

This project demonstrates practical experience in:

* Data cleaning and transformation
* Exploratory data analysis
* KPI development
* DAX calculations
* Power BI dashboard development
* Data visualization
* Business-oriented analysis
* Web analytics
* Trend analysis
* Channel performance analysis
* Device performance analysis

---

## Key Analytical Metrics

| Metric               | Description                                  |
| -------------------- | -------------------------------------------- |
| Sessions             | Number of website sessions                   |
| Pageviews            | Total pages viewed                           |
| Unique Pageviews     | Number of unique page views                  |
| Bounce Rate          | Percentage of sessions that bounced          |
| Exit Rate            | Percentage of pageviews resulting in an exit |
| Pages per Session    | Average number of pages viewed per session   |
| Average Time on Page | Average time users spent on a page           |

---

## Project Outcome

The final Power BI dashboard provides an interactive view of website marketing performance and enables users to analyze traffic, engagement, acquisition channels, devices, countries, and content performance.

The project demonstrates how raw web analytics data can be transformed into meaningful business insights using Power BI and DAX.
# Web-Marketing-Performance-Analysis
Web Marketing Performance Analysis using Power BI, DAX, Power Query and Excel
