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


