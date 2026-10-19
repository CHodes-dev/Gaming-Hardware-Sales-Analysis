# Exploratory Data Analysis

## Introduction

Once the data has been cleaned so that it is ready for analysis, the next step is to carry out exploratory data analysis. One aspect that must not be overlooked when undertaking a data analysis project is **Requirements gathering**.
Requirements gathering is a preventative method to avoid aimless analysis in an EDA project. It involves narrowing down the scope and taking a planned approach to defining what the expected outcomes should be.

The process for gathering requirements begins with:
1. Defining metrics
2. Defining dimensions
3. Defining the desired outcomes

Thus, the following requirements were obtained for this project:
1. Metrics: Revenue, average order value (AOV), dan order count.
2. Dimensions: time, product, and region.
3. Outcomes: This report is intended for managers in other relevant teams.

The more detailed the explanation, the more focused the results will be.

Essentially, this Exploratory Data Analysis (EDA) phase aims to understand the data, identify specific trends, patterns, or anomalies, and determine whether the data can effectively answer the stakeholders' questions.

## EDA Framework

To starting EDA project, we can use the SCAN Framework:
**S - Stakeholder goals**: define KPIs and relevant dimensions.

**C - Columns and coverage**: determine what information can be derived from the available data.

**A - Aggregates and anomalies**: identify key metrics, outliers, and unexpected patterns.

**N - Notable segments**: group data by category, time, or other dimensions to uncover initial insights.

## EDA Process

Analysis scope based on the SCAN Framework.
Stakeholder goals
  - No decisions have been made yet based on high-level trends and patterns.
  - The important KPI is the revenue (Total of USD_PRICE).

Column and coverage
  - Uses the columns: USD_PRICE, PRODUCT_NAME, PURCHASE_TS

Aggregate and anomalies
  - Metric: USD_PRICE
  - Dimensions: PURCHASE_TS, PRODUCT_NAME
  - Identify: Min, Max, and Outliers

Notable segments
  - Other dimensions: REGION, MARKETING_CHANNEL, ACCOUNT_CREATION

**Initial Insights**

Below are some initial findings obtained after conducting an analysis in Excel, utilizing pivot tables, conditional formatting (color scales), and sparklines.

| Metric - Dimension | Insight | Relevant Team |
| --- | --- | --- |
| USD_PRICE - PURCHASE_TS | Total sales from 2019 to 2022 amounted to approximately $6.1M, with monthly sales ranging from $80K to $500K. | Finance |
| USD_PRICE - PRODUCT_NAME | - The product with the best sales performance is the 27-inch 4K gaming monitor, reaching $2M. - The product with the worst sales performance is the Razer Pro Gaming Headset, with a total of $800K. - It is necessary to check for missing values ​​in the sales data in coordination with the relevant team. | Finance, Product |
| USD_PRICE - PRODUCT_NAME| Gaming headset products (JBL Quantum 100 Gaming Headset & Razer Pro Gaming Headset) only contribute approximately 2% of total sales. | Product |
| USD_PRICE - PURCHASE_TS | A significant surge in sales occurred in December 2020. The Fall-Winter season, leading up to the new year, was recorded as the period with the best performance. | Marketing |
| USD_PRICE - PRODUCT_NAME | - All product types experienced a significant increase in sales from 2020 onwards, following the overall sales trend. - There was a macro-level or company-wide impact (initially presumed to be caused by COVID). | Finance |
| USD_PRICE - PRODUCT_NAME | Almost all products experienced a surge in sales in December 2020; it is worth examining the promotions or campaigns that took place during that period. | Marketing |
