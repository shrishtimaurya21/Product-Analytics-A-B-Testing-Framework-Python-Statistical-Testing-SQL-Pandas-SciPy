# 🚀 Product Analytics & A/B Testing Framework

## Overview

This project is an end-to-end Product Analytics and Experimentation Framework that simulates how modern product companies optimize user experiences using data-driven decision-making.

The project covers the complete experimentation lifecycle, including:

* User Funnel Analysis
* A/B Testing
* Statistical Significance Testing
* Sample Size Calculation
* Customer Cohort Analysis
* Multi-Touch Attribution Modeling
* Product KPI Monitoring
* Interactive Power BI Dashboarding

The framework enables product managers, growth teams, and data analysts to evaluate product changes, understand user behavior, and measure business impact through controlled experiments.

---

## Business Problem

Product teams frequently introduce new features, UI improvements, and checkout optimizations. Without proper experimentation and analytics, it becomes difficult to determine whether these changes improve key business metrics.

This project solves that problem by providing a complete experimentation framework capable of:

* Measuring conversion uplift
* Detecting statistically significant results
* Identifying funnel bottlenecks
* Tracking user retention
* Evaluating marketing channel performance
* Supporting data-driven product decisions

---

## Project Objectives

* Design a scalable A/B testing framework.
* Calculate statistically valid sample sizes.
* Randomly assign users into Control and Treatment groups.
* Perform hypothesis testing using real statistical methods.
* Analyze user conversion funnels.
* Build customer retention cohorts.
* Develop attribution models for acquisition channels.
* Create an executive dashboard for experiment monitoring.

---

## Tech Stack

| Technology  | Purpose                            |
| ----------- | ---------------------------------- |
| Python      | Analytics & Experimentation        |
| SQL         | Data Extraction & Aggregation      |
| Pandas      | Data Processing                    |
| NumPy       | Numerical Computing                |
| SciPy       | Statistical Testing                |
| Statsmodels | Power Analysis & Experiment Design |
| Power BI    | Dashboarding & Visualization       |
| DAX         | KPI Calculations                   |
| Excel       | Data Validation                    |

---

## Project Architecture

```text
Raw User Data
      │
      ▼
SQL Data Processing
      │
      ▼
Python Analytics Pipeline
      │
      ├── Sample Size Calculation
      ├── Randomization
      ├── Funnel Analysis
      ├── A/B Testing
      ├── Attribution Modeling
      └── Cohort Retention Analysis
      │
      ▼
Power BI Dashboard
      │
      ▼
Business Insights & Decision Making
```

---

## Project Structure

```text
product-analytics-ab-testing/
│
├── data/
│   ├── user_sessions.csv
│   ├── transactions.csv
│   ├── marketing_channels.csv
│   └── experiment_data.csv
│
├── sql/
│   ├── schema.sql
│   ├── funnel_analysis.sql
│   ├── attribution_model.sql
│   └── cohort_retention.sql
│
├── src/
│   ├── sample_size_calculator.py
│   ├── randomization.py
│   ├── funnel_analysis.py
│   ├── ab_test.py
│   ├── attribution.py
│   ├── cohort_analysis.py
│   └── dashboard_data.py
│
├── dashboard/
│   └── Product_Analytics.pbix
│
├── outputs/
│   ├── experiment_results.csv
│   ├── funnel_metrics.csv
│   ├── attribution_results.csv
│   └── cohort_retention.csv
│
├── notebooks/
│   └── product_analytics.ipynb
│
├── requirements.txt
├── main.py
└── README.md
```

---

## Dataset Description

### User Sessions Dataset

Contains user interactions across different stages of the product journey.

| Column    |
| --------- |
| UserID    |
| SessionID |
| Stage     |
| Device    |
| Channel   |
| Timestamp |

---

### Experiment Dataset

Stores experiment assignments and conversion outcomes.

| Column    |
| --------- |
| UserID    |
| Variant   |
| Converted |

---

### Marketing Dataset

Contains acquisition channel information.

| Column  |
| ------- |
| UserID  |
| Channel |
| Revenue |

---

### Transactions Dataset

Contains customer purchase history.

| Column    |
| --------- |
| UserID    |
| OrderID   |
| OrderDate |
| Revenue   |

---

# Key Features

---

## 1. Sample Size Calculation

Determines the minimum number of users required to achieve:

* Confidence Level: 95%
* Significance Level (α): 0.05
* Statistical Power: 80%

Benefits:

* Prevents underpowered experiments
* Reduces false conclusions

---

## 2. User Randomization

Randomly assigns users into:

* Control Group
* Treatment Group

Ensures unbiased experiment results.

---

## 3. Funnel Analysis

Tracks user progression through key stages:

```text
Landing Page
    ↓
Product Page
    ↓
Cart
    ↓
Payment
    ↓
Purchase
```

Metrics Generated:

* Stage Conversion Rate
* Drop-Off Rate
* Funnel Efficiency

---

## 4. A/B Testing Framework

Compares:

### Control Version

Current user experience

### Treatment Version

New product or UI variation

Statistical Tests:

* Chi-Square Test
* P-Value Analysis
* Statistical Significance Detection

Example Output:

```text
Control Conversion Rate: 12.3%

Treatment Conversion Rate: 13.7%

Conversion Uplift: 11.4%

P-Value: 0.008

Result:
Statistically Significant
```

---

## 5. Attribution Modeling

Measures the contribution of marketing channels.

Supported Models:

* First Touch Attribution
* Last Touch Attribution
* Linear Attribution
* Revenue Contribution Analysis

Business Impact:

* Marketing Budget Optimization
* Channel Performance Measurement

---

## 6. Cohort Retention Analysis

Tracks customer retention over time.

Metrics:

* Day 1 Retention
* Day 7 Retention
* Day 30 Retention
* Monthly Retention Curves

Insights:

* User Loyalty
* Product Stickiness
* Long-Term Engagement

---

## Power BI Dashboard

### Executive Overview

* Total Users
* Total Revenue
* Conversion Rate
* Experiment Uplift
* Statistical Significance

---

### Funnel Analytics

* Funnel Conversion
* Stage Drop-Off
* Checkout Performance

---

### Experiment Monitoring

* Control vs Treatment
* Conversion Lift
* P-Values
* Confidence Intervals

---

### Attribution Dashboard

* Revenue by Channel
* Attribution Breakdown
* Marketing ROI

---

### Cohort Dashboard

* Retention Heatmap
* Cohort Curves
* User Lifetime Trends

---

## Example Business Insights

This framework can answer questions such as:

* Which checkout design converts better?
* Where are users dropping off in the funnel?
* Which acquisition channels drive the most revenue?
* Which channels produce the most loyal customers?
* How long do users remain active after acquisition?
* Is the experiment statistically significant?

---

## Running the Project

### Clone Repository

```bash
git clone https://github.com/yourusername/product-analytics-ab-testing.git
```

### Navigate to Project Directory

```bash
cd product-analytics-ab-testing
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Execute Full Analytics Pipeline

```bash
python main.py
```

---

## Generated Outputs

```text
outputs/

├── experiment_results.csv
├── funnel_metrics.csv
├── attribution_results.csv
└── cohort_retention.csv
```

---

## Business Value Delivered

* Improved product decision-making through experimentation.
* Identified funnel bottlenecks affecting conversion.
* Measured statistical significance of product changes.
* Quantified acquisition channel effectiveness.
* Tracked customer retention and engagement trends.
* Enabled self-service analytics through dashboards.

---

## Future Enhancements

* Bayesian A/B Testing
* Sequential Testing
* CUPED Variance Reduction
* Multi-Armed Bandit Optimization
* Real-Time Experiment Monitoring
* Streamlit Experiment Dashboard
* Automated Experiment Report Generation
* Customer Lifetime Value Prediction

---

## Skills Demonstrated

* Product Analytics
* Experiment Design
* Statistical Testing
* Hypothesis Validation
* SQL Analytics
* Funnel Analysis
* Cohort Analysis
* Attribution Modeling
* Data Visualization
* Power BI Dashboarding
* Business Intelligence

---

## Author

**Shrashti Maurya**

B.Tech – Computer Science Engineering

Aspiring Data Analyst | Product Analyst | Business Analyst

Skills: Python, SQL, Power BI, Statistics, Machine Learning, Data Analytics

---

## License

This project is licensed under the MIT License.
