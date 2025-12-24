# Tailwind Traders – Power BI Business Analytics Project

## Business Context

Tailwind Traders is a retail business operating across multiple countries and product categories.
The leadership team requires clear visibility into sales performance, profitability, and customer
engagement in order to make informed business decisions.

This project focuses on building an end-to-end analytics solution using Power BI to transform
raw sales data into reliable, decision-ready insights through proper data preparation,
data modeling, analysis, and reporting.

## Project Objectives

The objective of this project was to design a business-ready analytics solution that enables
stakeholders to monitor sales performance and profitability across products, countries,
and time periods.

Specifically, the project aimed to:
- Prepare and validate raw sales data for analysis
- Build a structured and scalable data model in Power BI
- Define meaningful business metrics such as revenue and profit margin
- Create interactive reports to analyze trends and performance
- Deliver insights in a format suitable for executive decision-making

## Project Structure

The repository is organized to reflect how analytics projects are structured in
professional environments, with a clear separation between data, reports,
documentation, and outputs.

data/
- raw/        → Original, unmodified datasets as received
- processed/  → Enriched Sales dataset prepared for analysis

powerbi/
- reports/    → Power BI report (.pbix) containing data model, DAX, and visuals
- dashboard/  → Executive dashboard notes and references from Power BI Service

documentation/
- Explanations of assumptions, data modeling decisions, and metric definitions

screenshots/
- Visual previews of reports, dashboards, and data model

## Data Preparation & Modeling

Before building reports or dashboards, the focus was on ensuring that the data
was accurate, consistent, and structured correctly for analysis.

Sales data was initially prepared in Excel to validate business logic and
calculate essential financial fields such as revenue, tax, and profit.
This early preparation helped confirm that the numbers made sense before
moving into Power BI.

Multiple datasets, including sales, purchases, countries, and historical exchange
rates, were then integrated in Power BI. Historical exchange data was imported
using a Python script within Power Query, allowing currency conversion logic to
be handled during data ingestion rather than at the reporting layer. Data types 
were validated, relationships were defined, and a calendar table was introduced 
to ensure accurate time-based analysis

To enable consistent financial comparison across regions, all monetary values
were standardized into a single currency. The resulting data model was designed
to support scalable analysis across products, countries, and time periods.

> **Note:** This project is based on a retail business scenario and was developed as part of a
professional analytics capstone for learning and portfolio purposes.


