# khush
Work I have completed as a intern

Week 1 — Enterprise Data Discovery, Profiling & Business Readiness
Overview
During Week 1, I completed the initial Enterprise Data Discovery, Data Profiling, Relationship Analysis, Exploratory Data Analysis, KPI Foundation, SQL/DuckDB Query Development, Dashboard Discovery, and Data-Quality Assessment across the five core datasets:

•	Customers
•	Transactions
•	Products
•	Customer Support
•	Marketing Campaigns

The objective was to understand the structure, quality, relationships, and business usability of the available data before moving into deeper analytical and machine-learning activities.
________________________________________
Task 1 — Enterprise Data Profiling
Profiled all five datasets to establish an initial understanding of the available data.
Activities Completed

•	Recorded row and column counts for all five datasets.
•	Audited data types for every column.
•	Analyzed missing and null-value patterns.
•	Identified duplicate records and duplicate identifiers.
•	Checked column cardinality and uniqueness.
•	Identified potential primary keys and foreign keys.
•	Reviewed identifier consistency across datasets.
•	Documented data-quality anomalies in the shared Data-Quality Register.
•	Reviewed date fields, categorical fields, numerical fields, and identifier columns.

Datasets Profiled
Dataset	Profiling Performed
Customers	Structure, data types, nulls, duplicates, cardinality, identifiers
Transactions	Structure, revenue fields, status, dates, duplicates, identifiers
Products	Product identifiers, categories, numerical attributes, cardinality
Customer Support	Ticket identifiers, customer/transaction references, CSAT, response time
Marketing Campaigns	Campaign identifiers, customer references, spend, channels and outcomes
________________________________________
Task 2 — Data Relationship Analysis

Built an initial entity-relationship understanding across the five datasets.
Key Identifiers Reviewed

•	customer_id
•	product_id
•	transaction_id
•	Support identifiers such as ticket_id
•	Campaign identifiers
•	Other relevant business identifiers
Relationship Analysis Performed
•	Identified potential primary keys.
•	Identified potential foreign keys.
•	Checked customer-to-transaction relationships.
•	Checked product-to-transaction relationships.
•	Checked customer-to-support relationships.
•	Checked transaction-to-support relationships.
•	Reviewed customer-to-campaign relationships.
•	Identified missing relationships and orphan records.
•	Checked duplicate identifiers.
•	Reviewed referential-integrity concerns.

Marketing Campaigns
The relationship analysis provides the foundation for creating the integrated analytical dataset in the subsequent phase.
________________________________________
Task 3 — Exploratory Data Analysis

Conducted initial EDA to understand customer behaviour, transaction activity, product performance, customer-support activity, and marketing performance.

Customer Analysis
Analyzed:
•	Customer distribution.
•	Customer segments.
•	Order frequency.
•	Customer activity.
•	Purchase behaviour.
•	Recency and activity patterns.

Transaction Analysis
Analyzed:
•	Revenue distribution.
•	Transaction volume.
•	Order frequency.
•	Average transaction value.
•	Transaction status.
•	Return behaviour.
•	Revenue-related anomalies.

Product Analysis
Analyzed:
•	Product distribution.
•	Category distribution.
•	Product-level transaction activity.
•	Product contribution to transaction activity.

Customer Support Analysis
Analyzed:
•	Ticket distribution.
•	Issue categories.
•	CSAT patterns.
•	Response-time patterns.
•	Customer and transaction references within support data.

Marketing Analysis
Analyzed:
•	Campaign spend.
•	Revenue generated.
•	Marketing channels.
•	Channel-level performance.
•	Initial ROI observations.
•	Customer/campaign relationships.
The EDA was used to identify important patterns and potential areas requiring deeper analysis in later weeks.
________________________________________
Task 4 — Business KPI Foundation
Created an initial KPI dictionary for the major business metrics required for enterprise reporting and dashboard development.
KPIs Defined

1.	Total Revenue
2.	Average Order Value
3.	Repeat Purchase Rate
4.	Return Rate
5.	Attrition Risk Rate
6.	CSAT
7.	Campaign ROI
8.	Support SLA Breach Rate
   
For each KPI, the following were documented:
•	Business definition.
•	Calculation/formula.
•	Data source.
•	Required filters.
•	Business owner.
•	Expected refresh frequency.
•	Data dependencies.
•	Validation considerations.

The KPI foundation establishes consistent metric definitions before dashboard development and executive reporting.
________________________________________
Task 5 — SQL / DuckDB Query Foundation

Created the initial SQL/DuckDB exploratory query bank to validate the business data and support analytical requirements.
Query Areas Covered

•	Revenue analysis.
•	Customer analysis.
•	Product analysis.
•	Transaction analysis.
•	Customer-support analysis.
•	Marketing campaign analysis.
•	Regional performance.
•	Customer activity.

Week 1 Validation
At least 8 exploratory SQL/DuckDB queries were developed and validated during Week 1.

The queries were used to:
•	Validate dataset structure.
•	Check business metrics.
•	Investigate data-quality issues.
•	Analyze transaction and customer behaviour.
•	Validate relationships between entities.
•	Support the initial KPI definitions.
________________________________________
Task 6 — Dashboard Discovery

Created initial dashboard concepts and wireframes for three enterprise analytical dashboards.
Dashboard 1 — Enterprise Revenue Command Center

Intended KPIs
•	Total Revenue
•	Average Order Value
•	Total Orders
•	Repeat Purchase Rate
•	Return Rate
•	Customer Count

Filters
•	Date
•	Region
•	Product Category
•	Customer Segment
•	Transaction Status

Dimensions
•	Time
•	Region
•	Product Category
•	Customer Segment
•	Product

Drilldowns
Enterprise
   ↓
Region
   ↓
Customer Segment
   ↓
Customer / Product
   ↓
Transaction Detail

User Persona
•	Business Leadership
•	Sales Leadership
•	Revenue Management
•	Business Analysts

Business Questions
•	How is revenue performing?
•	Which regions contribute most to revenue?
•	Which product categories drive transaction activity?
•	How does revenue vary across customer segments?
•	What is the return behaviour?
________________________________________
Dashboard 2 — Customer Retention & Lifetime Value Cockpit

Intended KPIs
•	Total Customers
•	Average Customer Lifetime Value
•	Repeat Purchase Rate
•	Dormant Customer Rate
•	Attrition Risk Rate
•	High-Value Customer Count

Filters
•	Date
•	Region
•	Customer Segment
•	Customer Risk
•	Product Category
•	Tenure

Dimensions
•	Customer Segment
•	Region
•	Customer Lifecycle
•	Tenure
•	Product Category

Business Questions
•	Which customers are active or dormant?
•	Which customer groups have high lifetime value?
•	What is the repeat-purchase behaviour?
•	Which customer populations require further investigation?
•	How does customer activity vary by region and segment?
________________________________________
Dashboard 3 — Marketing & Service Excellence Dashboard

Intended KPIs
•	Campaign Spend
•	Campaign Revenue
•	Campaign ROI
•	Campaign Performance
•	CSAT
•	Average Response Time
•	Support SLA Breach Rate
•	Ticket Volume

Filters
•	Date
•	Marketing Channel
•	Campaign
•	Region
•	Customer Segment
•	Issue Type
•	Support Status

Dimensions
•	Campaign
•	Marketing Channel
•	Region
•	Customer Segment
•	Issue Type
•	Support Agent

Business Questions
•	Which channels generate revenue?
•	What is the relationship between campaign spend and generated revenue?
•	Which support issues occur most frequently?
•	How does CSAT vary across support activity?
•	Where are response-time or SLA concerns observed?

The dashboards were treated as initial discovery wireframes rather than production-complete dashboards.
________________________________________
Task 7 — Data-Quality & Business Readiness Memo

Prepared an initial business-readiness assessment covering the major data-quality and business-definition risks.
Areas Assessed
Null-Value Patterns
Reviewed missing values across all five datasets and identified fields requiring validation, treatment, or business rules before downstream analysis.
Date Inconsistencies

Reviewed transaction, customer, support, and campaign date fields for:
•	Missing dates.
•	Invalid date values.
•	Date-format consistency.
•	Chronological inconsistencies.

Duplicate Records
Reviewed datasets for:
•	Fully duplicated rows.
•	Duplicate business identifiers.
•	Potential duplicate transactions.
•	Duplicate customer/product/support/campaign identifiers.

Status Inconsistencies
Reviewed transaction and support status fields for inconsistent or unexpected categorical values.
Identifier Issues
Reviewed:
•	customer_id
•	product_id
•	transaction_id
•	ticket_id
•	Campaign identifiers
for missing, duplicated, unmatched, or orphaned references.

Revenue Filtering Rules
Established the need for clearly defined revenue treatment before executive reporting, including:
•	Which transaction statuses are included.
•	Whether returned transactions are excluded or separately reported.
•	Treatment of cancelled transactions.
•	Treatment of invalid or incomplete transaction records.
Returned / Cancelled Transactions
Returned and cancelled transactions were identified as important business-rule considerations.
Rather than treating them automatically as normal revenue, their treatment should be explicitly defined and consistently applied across SQL, Python, and Power BI calculations.
________________________________________
Week 1 Outcome
Week 1 established the data discovery and analytical foundation required for the next phase of the project.
Completed Deliverables

•	Enterprise data profiling.
•	Data-quality assessment.
•	Entity and relationship analysis.
•	Referential-integrity checks.
•	Initial exploratory data analysis.
•	KPI dictionary.
•	SQL/DuckDB exploratory query bank.
•	Initial dashboard wireframes.
•	Business-readiness assessment.
•	Data-quality register.
Next Phase
The findings from Week 1 will be used to support Week 2 activities, including:
•	Data cleaning and standardization.
•	Integrated/master analytical dataset creation.
•	Customer feature engineering.
•	KPI activation and validation.
•	Revenue Command Center development.
•	Return and discount analysis.
•	Marketing performance analysis.
•	Improved data-quality controls.

----------------------------------------------------------------------------------------------------------------------------

# Week 2 

## Overview

During Week 2, I developed a reproducible data preparation and analytical workflow for the VANTAGE360 datasets. The work focused on transforming the raw enterprise datasets into standardized, governed, and analysis-ready data while establishing the foundation for customer intelligence, revenue analytics, KPI reporting, and dashboard development.

The five core datasets used were:

- Customers
- Transactions
- Products
- Customer Support
- Marketing Campaigns

The completed work covered data cleaning, master analytical dataset creation, customer feature engineering, attrition analysis, KPI activation, SQL query development, return and discount analysis, campaign staging, dashboard development, validation, and executive insights.

---

#  Automated Data Cleaning Pipeline

Developed a reproducible data-cleaning pipeline for the VANTAGE360 datasets.

### Data Preparation Activities Completed

- Identified missing values across all datasets.
- Applied appropriate missing-value treatment based on field type and business meaning.
- Detected duplicate records.
- Handled duplicate records according to the relevant business identifiers.
- Normalized data types.
- Standardized date and time fields.
- Validated currency and numerical fields.
- Standardized categorical values.
- Detected invalid transaction records.
- Performed negative and zero-value checks where applicable.
- Validated referential integrity.
- Checked customer ID consistency.
- Checked product ID consistency.
- Validated transaction status values.
- Standardized column names and formats.

The pipeline was designed to be **reproducible and reusable**, avoiding manual spreadsheet-based data cleaning.

### Output

The cleaning workflow produces standardized datasets that can be directly consumed by SQL, Python, Power BI, and downstream analytical processes.

---

# Master Analytical Dataset

Created a consolidated analytical data foundation by integrating the major business entities:

- Customers
- Transactions
- Products
- Customer Support
- Marketing Campaigns

The datasets were integrated using business relationships rather than simply concatenating the raw tables.

### Documented Components

- Dataset grain.
- Primary identifiers.
- Foreign-key relationships.
- Join logic.
- Aggregation logic.
- Derived analytical fields.
- Missing-value treatment.
- Business assumptions.
- Referential-integrity considerations.

The resulting structure provides a foundation for customer-level, transaction-level, product-level, support-level, and campaign-level analysis.

---

# Customer Feature Foundation

Created a customer-level analytical feature table to support customer intelligence, segmentation, retention analysis, and future ML activities.

## Customer Activity Features

Created or investigated:

- Total orders.
- Total revenue.
- Average Order Value.
- First purchase date.
- Last purchase date.
- Purchase frequency.
- Days since last purchase.
- Purchase recency.

## Customer Value Features

Created or investigated:

- Lifetime revenue.
- Average transaction value.
- Revenue contribution.
- Product-category diversity.
- Purchase frequency.

## Customer Engagement Features

Integrated or analyzed:

- Support interactions.
- Campaign interactions where available.
- Return behaviour.
- Purchase recency.
- Purchase consistency.

## Customer Status

Created business-oriented customer classifications:

- Premium
- Regular
- Occasional
- Dormant

The segmentation logic was documented using measurable business rules rather than assigning segments without explanation.

The customer feature table provides the foundation for retention analysis, customer profiling, LTV analysis, and future predictive modelling.

---

# Customer Attrition / Churn Proxy

Developed a documented analytical proxy for customer attrition.

### Factors Investigated

- Last purchase recency.
- Historical purchase frequency.
- Customer tenure.
- Order count.
- Revenue history.
- Return behaviour.
- Support interactions.
- Campaign engagement where available.

A provisional inactivity/attrition rule was established for analytical purposes.

### Documentation Included

- Attrition proxy definition.
- Threshold/rule used.
- Business reasoning behind the threshold.
- Limitations of the proxy.
- Potential sources of false positives and false negatives.
- Approach for converting the proxy into a future supervised ML target.

The proxy is treated as an analytical indicator rather than a confirmed prediction of actual customer churn.

---

# Revenue Command Center Data Layer

Prepared the analytical data required for the Revenue Command Center.

### Revenue Analysis

Analyzed:

- Total revenue.
- Revenue by region.
- Revenue by product.
- Revenue by product category.
- Revenue by customer segment.
- Revenue by channel where available.
- Transaction volume.
- Average Order Value.
- Repeat purchase behaviour.
- Return rate.
- Discount impact.
- Revenue contribution by customer segment.

Major KPIs were linked back to governed SQL calculations to improve traceability and consistency between the analytical layer and dashboard layer.

---

# KPI Activation

Implemented and validated the project's core business KPIs.

## Core KPIs

### Total Revenue
Revenue generated from valid delivered transactions according to the agreed business rules.

### Average Order Value
Calculated using the defined revenue and valid order/transaction population.

### Repeat Purchase Rate
Percentage of customers who completed more than one qualifying purchase.

### Return Rate
Returned transactions divided by the relevant transaction population according to the defined business rule.

### Attrition Risk Rate
Percentage of customers meeting the documented inactivity/attrition proxy.

### Customer Value
Customer-level accumulated revenue supported by additional customer value metrics.

### KPI Documentation

Each KPI was documented with:

- Definition.
- SQL logic.
- Source tables.
- Required filters.
- Analytical grain.
- Validation result.
- Business interpretation.
- Relevant dependencies.

This created a consistent KPI foundation for Power BI and executive reporting.

---

# SQL Query Bank
Expanded the SQL/DuckDB query library to **15+ reusable business queries**.

## Revenue Queries

- Revenue by month.
- Revenue by region.
- Revenue by product.
- Top customers by revenue.
- Revenue contribution by customer segment.

## Customer Queries

- New customers.
- Repeat customers.
- Dormant customers.
- Customer purchase frequency.
- Customer lifetime value.

## Transaction Queries

- Average Order Value.
- Return analysis.
- Discount analysis.
- High-value transactions.
- Transaction trends.

## Business Intelligence Queries

- Regional performance.
- Product performance.
- Customer segment performance.
- Campaign-related revenue where supported.
- Support and customer-behaviour relationships.

The SQL queries were written to be readable, reproducible, and compatible with the project's SQL/DuckDB environment.

---

# Return & Discount Analysis
Conducted an analytical investigation into discounts, transaction outcomes, and return behaviour.

### Analysis Performed

- Discount distribution.
- Discount by product.
- Discount by customer segment.
- Discount versus order value.
- Discount versus return behaviour.
- Revenue after discount.
- High-discount customer groups.
- Return patterns across relevant transaction groups.

The analysis was used to identify business patterns and potential areas for management attention.

No causal conclusions were made where the available observational data could only establish association.

### Business Focus
The analysis considered whether discounting appears to be associated with:

- Higher transaction value.
- Different customer segments.
- Increased return behaviour.
- Changes in revenue quality.

---

# Campaign Staging Dataset

Prepared a clean campaign analysis dataset to support future marketing analytics.

### Intended Analytical Uses

- Campaign performance.
- Customer targeting.
- Campaign response.
- Revenue attribution.
- Customer segmentation.
- Campaign ROI.

### Relationship Analysis

Documented the supported relationship:

```text
Customer
   ↓
Campaign
   ↓
Transaction
   ↓
Revenue
```

Where direct attribution was not fully supported by the available identifiers, the limitation was documented rather than assuming an unsupported relationship.

---

# Dashboard — Revenue Command Center v1
Developed the first analytical version of the **Revenue Command Center**.

## Executive KPI Strip

Included:

- Revenue.
- Average Order Value.
- Orders.
- Repeat Purchase Rate.
- Return Rate.
- Customer Count.

## Revenue Analysis

Included:

- Revenue trend.
- Regional revenue.
- Product/category revenue.
- Segment revenue.

## Customer Analysis

Included:

- Premium customers.
- Regular customers.
- Occasional customers.
- Dormant customers.

## Transaction Analysis

Included:

- Returns.
- Discounts.
- Order trends.

The dashboard was structured to clearly distinguish between:

- KPI
- Trend
- Breakdown
- Business Insight

This allowed users to move from high-level performance monitoring to more detailed analytical investigation.

---

# Dashboard Drill-Through

Implemented drill-through functionality where technically supported.

The intended analytical flow was:

```text
Executive KPI
      ↓
Segment
      ↓
Customer / Product / Region
      ↓
Detailed Record
```

This design allows users to investigate the underlying drivers of KPI movements rather than using the dashboard only as a visual reporting tool.

---

# Analytical Validation

Performed reconciliation between:

- Source datasets.
- Cleaned datasets.
- SQL outputs.
- Dashboard outputs.

### Validation Process
Important KPI values were independently checked between the different analytical layers.

The validation covered metrics such as:

- Revenue.
- Orders.
- Customer count.
- Average Order Value.
- Repeat Purchase Rate.
- Return Rate.
- Segment-level revenue.
- Regional revenue.
- Customer-level revenue.
- Other major dashboard KPIs.

At least **10 important KPI values were reconciled**.

Any identified discrepancies were investigated and documented based on differences in:

- Filters.
- Transaction status.
- Data cleaning.
- Aggregation logic.
- Missing values.
- Join behaviour.
- KPI definitions.

This validation helped ensure consistency between the data layer, SQL calculations, and dashboard outputs.

---

#Executive Insight Brief
Prepared an executive-level analytical summary based on the completed analysis.

## Revenue
Reviewed overall revenue performance, revenue trends, regional contribution, product/category contribution, and customer-segment contribution.

## Customers
Analyzed customer segments and identified the customer groups contributing the largest share of business value based on revenue and purchase behaviour.

## Retention
Used purchase recency, order frequency, customer activity, and the attrition proxy to identify customer groups showing signs of reduced engagement or inactivity.

## Products
Analyzed product and category-level transaction activity and revenue contribution to identify stronger and weaker-performing areas.

## Regions
Compared regional revenue and customer activity to identify regions requiring additional investigation or management attention.

## Business Recommendations
Recommendations were structured using:

```text
Problem
   ↓
Evidence
   ↓
Business Impact
   ↓
Recommended Action
```

Recommendations were based on observed data patterns rather than generic statements.

Examples of analytical recommendation areas included:

- Targeted re-engagement of inactive customer groups.
- Segment-specific retention strategies.
- Investigation of high-return product/category patterns.
- Review of high-discount customer groups.
- Regional performance monitoring.
- Further investigation of campaign-to-revenue relationships.
- Improvement of support processes where response-time or CSAT patterns indicate potential service issues.

---

# Week 2 Key Deliverables

The following deliverables were completed during Week 2:

- Automated/reproducible data-cleaning pipeline.
- Standardized analytical datasets.
- Master Analytical Dataset.
- Customer Feature Foundation.
- Customer segmentation.
- Customer attrition/churn proxy.
- Revenue Command Center data layer.
- Core KPI activation.
- 15+ SQL/DuckDB business queries.
- Return and discount analysis.
- Campaign staging dataset.
- Revenue Command Center v1 dashboard.
- Dashboard drill-through structure.
- KPI reconciliation and validation.
- Executive Insight Brief.

---

# Week 2 Outcome

Week 2 transformed the raw enterprise data foundation established during Week 1 into a more **standardized, governed, and business-ready analytical environment**.

The completed work established the foundation for subsequent activities involving:

- Advanced customer analytics.
- Customer retention and LTV analysis.
- Predictive modelling.
- ML-based customer risk analysis.
- Campaign intelligence.
- Advanced Power BI dashboards.
- Next-best-action recommendations.
- Deeper executive decision support.

The overall workflow follows:

```text
Raw Enterprise Data
        ↓
Data Cleaning & Validation
        ↓
Standardized Datasets
        ↓
Master Analytical Dataset
        ↓
Customer Feature Foundation
        ↓
KPI Activation & SQL Validation
        ↓
Business Analysis
        ↓
Revenue Command Center
        ↓
Executive Insights
        ↓
Advanced Analytics & ML Foundation
```

This Week 2

# Week 3 — Deep Customer Analytics, Retention & LTV Intelligence

## Overview

During Week 3, I developed a deeper customer analytics layer focused on **retention, customer lifetime value (LTV), lifecycle segmentation, cohort analysis, regional retention, customer risk, product affinity, and retention opportunities**.

The analysis extended the Week 2 customer feature foundation and transformed it into a customer-level intelligence layer suitable for business decision-making and future ML use cases.

The major areas covered were:

- Customer Retention & LTV Intelligence
- Customer Lifecycle Segmentation
- Cohort Retention Analysis
- Regional Retention Analysis
- High-Value Customer Risk Analysis
- Retention & LTV Dashboard
- SQL Business Query Expansion
- ML Risk Reconciliation
- Customer Risk Analysis
- Retention Opportunity Analysis
- Product & Customer Affinity
- Next-Best-Action Data Preparation
- Executive Retention Story

----------------------------------------------------------------------------------------
week 3-


# Retention & LTV Intelligence
Developed a customer-level analytical layer focused on understanding customer value and retention behaviour.

## Customer Value & Retention Metrics

Analyzed and created features for:

- Customer lifetime revenue.
- Customer tenure.
- Total orders.
- Purchase frequency.
- Purchase recency.
- Average Order Value.
- Repeat purchase behaviour.
- Product-category diversity.
- Return behaviour.
- Discount behaviour.
- Customer support interactions.
- Campaign interactions where available.

## Customer-Level Analytical Table

Created a customer-level feature table containing the major retention and LTV metrics.

The table provides a consolidated view of:

```text
Customer
   ↓
Purchase Behaviour
   ↓
Customer Value
   ↓
Engagement
   ↓
Retention Behaviour
   ↓
Risk Indicators
```

This table was designed to support retention analysis, customer segmentation, risk identification, and future machine-learning activities.

# Customer Lifecycle Segmentation
Expanded the Week 2 customer segmentation into a detailed lifecycle view.

## Customer Segments
Customers with high business value and significant revenue contribution based on the documented segmentation methodology.

### Regular
Customers demonstrating established and relatively consistent purchasing activity.

### Occasional
Customers with comparatively limited purchase activity.

### Dormant
Customers showing prolonged inactivity based on the documented recency/inactivity threshold.

## Segmentation Methodology
The segmentation methodology was documented using measurable customer attributes such as:

- Revenue.
- Order count.
- Purchase recency.
- Purchase frequency.
- Customer activity.
- Business value.

The thresholds were defined using the project's documented business rules rather than assigning labels arbitrarily.

## Segment Analysis
For each segment, analyzed:

- Number of customers.
- Revenue contribution.
- Regional distribution.
- Average LTV.
- Average purchase recency.
- Purchase behaviour.
- Customer activity.

This provided a clearer understanding of the composition and value of each customer lifecycle group.


# Retention Cohort Analysis
Performed cohort analysis using customer signup or first-purchase date where supported by the available data.

## Retention Periods

Analyzed:

- Month 0 retention.
- Month 1 retention.
- Month 2 retention.
- Month 3 retention.
- Longer-term retention where sufficient data was available.

## Cohort Outputs
Created:

- Cohort retention table.
- Retention percentages by cohort.
- Retention curve.
- Cohort comparison analysis.

The analysis was used to compare retention behaviour across different customer acquisition/first-purchase cohorts and identify differences in longer-term customer engagement.

# Regional Retention Analysis
Conducted regional customer-retention analysis.

For each region, calculated and analyzed:

- Customer count.
- Revenue.
- Average Order Value.
- Repeat Purchase Rate.
- Dormant Customer Rate.
- Attrition Proxy Rate.
- Average LTV.
- High-value customer count.

## Regional Analysis
Regional performance was compared across customer value, retention, activity, and risk indicators.

The analysis helped identify:

- Regions with stronger customer retention and value.
- Regions with higher inactivity or attrition-proxy levels.
- Regions containing significant high-value customer populations.
- Areas requiring additional business investigation.

An executive summary was prepared to explain the observed differences using the available evidence.

# High-Value Customer Risk Analysis
Combined customer value and customer activity/risk indicators to identify strategically important customer populations.

A major focus was:

text
High LTV + High Attrition Risk

## Priority Populations

### Priority 1

**High LTV + High Risk**
High-value customers showing strong indicators of inactivity or attrition risk.

### Priority 2

**High LTV + Medium Risk**
High-value customers showing moderate risk indicators.

### Priority 3

**Medium LTV + High Risk**
Customers with meaningful business value and elevated risk indicators.

The thresholds were based on the team's documented business definitions.

This analysis created a prioritized customer population for retention investigation.

# DA-06 — Retention & LTV Cockpit
Developed the second major analytical dashboard: **Retention & LTV Cockpit**.

## Executive KPIs
The dashboard included:

- Total Customers.
- Average LTV.
- Repeat Purchase Rate.
- Dormant Customer Rate.
- Attrition Risk Rate.
- High-Value Customer Count.

## Customer Segmentation
Analyzed:

- Premium.
- Regular.
- Occasional.
- Dormant.

## Retention Analysis
Included:

- Cohort retention.
- Retention trend.
- Regional retention.
- Customer lifecycle analysis.

## Risk Analysis
Included:

- High-risk customers.
- High-risk regions.
- High-value/high-risk customers.
- Customer risk distribution.

## LTV Analysis
Included:

- LTV distribution.
- LTV by region.
- LTV by customer segment.
- Top customers by LTV.

The dashboard was designed to move from executive-level KPIs to customer-level investigation.

# SQL Query Bank Expansion
Expanded the SQL business query library to **20+ reusable analytical queries**.

## Retention Queries
Included queries for:

- Cohort retention.
- Dormant customers.
- Repeat customers.
- Retention by region.
- Retention by customer segment.

## LTV Queries
Included:

- Customer lifetime revenue.
- Average LTV.
- LTV by region.
- LTV by customer segment.
- Top customers by LTV.

## Risk Queries
Included:

- High-risk customers.
- High-value/high-risk customers.
- Risk by region.
- Risk by customer segment.

## Behavioral Intelligence Queries
Included:

- Purchase frequency.
- Product diversity.
- Discount behaviour.
- Return behaviour.
- Support interaction patterns.

The SQL query bank was designed to remain readable, reusable, and compatible with the project's SQL/DuckDB analytical 

# ML Risk Reconciliation
Performed analytical validation of the ML-generated customer risk outputs provided by the ML track.

The objective was to compare model-generated risk indicators against observed customer behaviour.

## Comparisons Performed

Analyzed:

- ML Risk Score versus actual customer behaviour.
- High-risk customers with recent purchases.
- Low-risk customers with prolonged inactivity.
- High-value customers receiving high-risk scores.
- Segment-level risk distribution.
- Regional risk distribution.

## Validation Focus
The analysis did not attempt to prove that the ML model was correct or incorrect.

Instead, it investigated:

- Areas of agreement.
- Areas of disagreement.
- Unexpected patterns.
- Potential data-quality issues.
- Potential model limitations.
- Customer segments requiring further investigation.

This provided a business-oriented reconciliation layer between model output and observed customer behaviour.

# Customer Risk Dashboard
Created an analytical view focused specifically on customer risk.

## Dashboard Components
Included:

- Risk distribution.
- Risk by region.
- Risk by customer segment.
- Risk by LTV.
- High-value/high-risk customers.
- Risk-factor analysis.
- Customer-level drill-down.

## Investigation Flow
The dashboard was designed around:

text
Risk KPI
   ↓
Region
   ↓
Customer Segment
   ↓
Customer
   ↓
Customer-Level Details
```

This allowed management users to investigate the customer populations contributing to observed risk levels.


# Customer Retention Opportunity Analysis
Identified actionable customer-retention opportunities based on customer value, activity, and behavioural signals.

## Opportunity Areas

### Opportunity A — High-LTV Customers
Identified high-LTV customers showing increasing purchase recency or reduced recent activity.

### Opportunity B — Premium Customers
Analyzed Premium customers showing declining purchase frequency.

### Opportunity C — Dormant High-Value Customers
Identified dormant customers with historically significant revenue contribution.

### Opportunity D — Regional Risk
Identified regions containing high-value customers alongside elevated attrition-risk indicators.

## Opportunity Framework
Each opportunity was documented using:

text
Customer Group
      ↓
Evidence
      ↓
Risk / Opportunity
      ↓
Recommended Business Action
```

Recommendations were based on observed customer behaviour rather than generic retention statements.

# Product & Customer Affinity Analysis
Investigated relationships between customers and products/categories.

## Analysis Performed
Analyzed:

- Most frequently purchased categories.
- Categories associated with high-LTV customers.
- Categories associated with repeat purchases.
- Category preferences by customer segment.
- Category behaviour among high-risk customers.

The analysis was used to understand customer-product relationships and provide supporting signals for future recommendation modelling.

# Next-Best-Action Data Preparation
Prepared analytical features that can support future customer recommendation and next-best-action modelling.

## Features Prepared / Investigated

- Customer segment.
- Purchase history.
- Product category.
- Last purchase date.
- Purchase frequency.
- Lifetime value.
- Discount behaviour.
- Return behaviour.
- Campaign interaction.
- Support history.

The features were documented to support future ML and recommendation activities.

The analytical structure provides a foundation for potential use cases such as:

- Retention offers.
- Re-engagement.
- Product recommendations.
- Upselling.
- Cross-selling.
- Customer-service interventions.

# Executive Retention Story
Prepared a Week 3 executive-level retention and customer-value story.

## Customer Value
Analyzed which customer segments and individual customers generate the greatest business value based on lifetime revenue, purchase behaviour, and LTV-related metrics.

## Retention
Analyzed customer activity, recency, repeat behaviour, dormant populations, and cohort retention to identify areas where retention requires attention.

## Risk
Identified customer groups with elevated attrition-risk indicators, particularly high-value customers with high risk.

## Regional Risk
Compared regional customer value and retention indicators to identify regions requiring further management attention.

## Opportunity
Prioritized customer populations based on the combination of:

- Customer value.
- Purchase activity.
- Recency.
- Attrition risk.
- Segment.
- Regional characteristics.

## Recommendation

Developed evidence-based recommendations using:

text
Business Problem
      ↓
Supporting Evidence
      ↓
Business Impact
      ↓
Recommended Action
```

The recommendations were designed to be specific to the observed customer behaviour rather than generic statements such as "improve customer retention."



# Week 3 Key Deliverables

The following analytical deliverables were completed during Week 3:

- Customer-level Retention & LTV analytical table.
- Customer lifetime revenue analysis.
- Customer tenure analysis.
- Purchase frequency and recency analysis.
- Repeat-purchase analysis.
- Product diversity analysis.
- Return and discount behaviour analysis.
- Support interaction analysis.
- Detailed customer lifecycle segmentation.
- Segment-level value and retention analysis.
- Cohort retention analysis.
- Regional retention analysis.
- High-value/high-risk customer analysis.
- Retention & LTV Cockpit.
- 20+ SQL business queries.
- ML risk reconciliation.
- Customer Risk Dashboard.
- Customer retention opportunity analysis.
- Product/customer affinity analysis.
- Next-best-action feature preparation.
- Executive Retention Story.

---

# Week 3 Analytical Flow

```text
Customer & Transaction Data
            ↓
Customer-Level Features
            ↓
Retention & LTV Metrics
            ↓
Lifecycle Segmentation
            ↓
Cohort & Regional Analysis
            ↓
Customer Risk Analysis
            ↓
High-Value / High-Risk Identification
            ↓
Retention Opportunities
            ↓
Dashboard & Executive Insights
            ↓
ML / Recommendation Foundation
```

# Week 3 Outcome

Week 3 expanded the VANTAGE360 analytical foundation from revenue and KPI reporting into **deeper customer intelligence**.

The completed work established a structured analytical layer for understanding:

- Who the highest-value customers are.
- How customers behave across their lifecycle.
- Which customers show signs of disengagement.
- How retention differs across cohorts and regions.
- Which high-value customers require closer attention.
- Which products and categories are associated with customer behaviour.
- Which customer features can support future ML and recommendation use cases.

This analytical foundation provides the basis for subsequent **predictive customer-risk modelling, recommendation systems, next-best-action strategies, and advanced customer decision support**.

