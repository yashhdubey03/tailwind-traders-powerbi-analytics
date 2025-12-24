# Documentation Overview

This folder contains the analytical and design decisions behind the Power BI
solution for the Tailwind Traders business scenario.

Rather than only showing the final dashboards, this documentation highlights
*why* certain choices were made during the project, reflecting a business-first
approach to analytics.

---

## Key Decisions & Rationale

### 1. Data Preparation in Excel
- Added revenue, tax, and profit columns to validate business logic before importing.
- Confirmed initial calculations matched expected behavior on sample records.
- Purpose: ensure the dataset was **business-ready** before modeling.

### 2. Currency Conversion Strategy
- Historical exchange data imported using a **Python script in Power Query**.
- Conversion applied **during ingestion**, not in report visuals.
- Purpose: standardize values to USD and avoid inconsistent calculations.

### 3. Data Modeling Approach
- Relationship design based on fact (Sales) + lookup (Countries, Exchange Rates).
- Calendar table added to support **time intelligence** functions (YTD, QTD, yearly metrics).
- Purpose: support reporting by product, geography, and time period **reliably**.

### 4. Metric Philosophy
- Used **Median Sales** instead of Average to avoid skew from outliers.
- Profit Margin tracked at **YTD, Quarterly, and Yearly** granularity.
- Purpose: answer stakeholder questions, not just create visuals.

---

## How This Supports the Business

| Business Need | Solution Implemented |
|---------------|-----------------------|
| Understand revenue trends | YTD + time-series visuals |
| Compare markets | Country-based segmentation |
| Identify best performers | Product ranking & KPIs |
| Proactive action | Alerts + Subscriptions |
| Executive monitoring | Service-level dashboard |

---

## Why This Documentation Exists

This documentation does *not* attempt to be technical notes or training
material. Instead, it exists to:

- Show clear analytical intent  
- Make the project defensible in interviews  
- Demonstrate decision-making skills  
- Help recruiters see **how** you think, not just what you built

---

> 📌 **If you're a reviewer:**  
> This folder is meant to give context, not instructions.  
> Please explore the repository root + README for the full narrative.
