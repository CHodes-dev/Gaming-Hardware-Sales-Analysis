# Gaming Hardware Sales Analysis

## Background

GameZone is a company that has been selling gaming hardware, both new and refurbished-worldwide through a variety of marketing channels, offline and online since 2018.

The company needs to understand sales performance during the COVID-19 pandemic, from 2019 to 2021. The results of this analysis are used to evaluate the performance of each team, enabling strategic decisions to be made to improve the company’s overall performance.

Insights and recommendations are available across several key areas:
- Sales trend analysis: evaluating historical sales patterns with a focus on revenue.
- Product performance: analysing various product lines to understand their impact on company revenue.
- Marketing channel performance: assessing the performance of each marketing channel to identify which generates the most revenue.
- Regional performance: evaluating sales by region.

The data used can be viewed [here](https://github.com/CHodes-dev/Gaming-Hardware-Sales-Analysis/tree/main/datasets).

The workflow and framework used can be viewed [here](https://github.com/CHodes-dev/Gaming-Hardware-Sales-Analysis/tree/main/docs/project_workflow).

The interactive Power BI dashboard can be downloaded [here](https://github.com/CHodes-dev/Gaming-Hardware-Sales-Analysis/blob/main/docs/gamezone_dashboard.pbix).

⚠️Heads up! This project is part of the ‘**Portfolio Playbook**’ series uploaded by Christine Jiang on her [YouTube channel](https://www.youtube.com/@christinejiangdata). The use of the dataset and framework also follows the material she has created. However, adjustments were still made.

## Data Structure

The company’s transaction data is contained in a single table comprising 21,864 rows, as shown below.

![structur_table](https://github.com/CHodes-dev/Gaming-Hardware-Sales-Analysis/blob/main/docs/images/data_structure.png)

## Executive Summary

![dashboard_preview](https://github.com/CHodes-dev/Gaming-Hardware-Sales-Analysis/blob/main/docs/images/preview_dashboard.png)

As can be seen from the graph in the dashboard above or [here](https://github.com/CHodes-dev/Gaming-Hardware-Sales-Analysis/blob/main/docs/gamezone_dashboard.pbix), the company’s revenue has increased significantly since the start of 2020 before eventually falling sharply towards the end of that year and into early 2021. This increase was observed across almost all product in all regions, indicating that the company’s performance was affected by the global COVID-19 pandemic, even after the surge in cases had subsided.

A more detailed analysis will be discussed below to identify the underlying causes and recommendations for action by each team within the company.

### 1. Sales Trend Analysis
- Total sales from 2019 to 2022 amounted to approximately $6.1M, with monthly sales ranging from $80K to $500K.
- Sales more than doubled in early 2020, peaking in September and December 2020. However, sales fell significantly from January 2021 onwards.

### 2. Product Performance
- The best-selling product was the 27-inch 4K gaming monitor, which generated $2 million.
- The worst-selling product was the Razer Pro Gaming Headset, with total sales of $800,000.
- The 27-inch 4K gaming monitor, the Nintendo Switch and the Sony PlayStation 5 bundle were the main causes of the decline in overall sales; all three showed a similar trend of plateauing in 2021.
- Gaming headsets (the JBL Quantum 100 Gaming Headset and the Razer Pro Gaming Headset) accounted for only around 2% of total sales.
- December 2020 saw a significant spike in sales. The autumn–winter season leading up to the New Year was recorded as the period with the strongest performance.

### 3. Marketing Channel Performance
- Direct sales are the main driver of high sales figures, whilst other marketing channels lag far behind.

### 4. Regional Performance
- All product saw a significant increase in sales from 2020 onwards, in line with the overall sales trend.
- All regions showed a similar decline in sales in 2021, indicating a global/macro trend.
- Almost all products experienced a surge in sales in December 2020; it is worth examining any promotions or campaigns that took place during that period.

### Recommendation

General
- As people spend more time at home, they will have a greater desire for entertainment, including purchasing gaming products.

Product Team
- Remove gaming headsets (JBL Quantum 100 Gaming Headset & Razer Pro Gaming Headset) from inventory as they contribute only 2% of overall revenue.

Marketing Team
- Focus on promoting the 27-inch 4K Gaming Monitor, Nintendo Switch and Lenovo IdeaPad Gaming 3 in North America as they show strong potential for appeal.
- Strengthen winter promotions by prioritising campaigns for the top 4 products in October or November.
- Focus marketing strategy on the email channel, which shows potential for growth, to reduce reliance on the direct channel.

Data Team
- Need to check for missing values in the sales data, particularly in the USD_PRICE field.
- Double-check that the attribution/source of data for these marketing channels is correct; the figures for the direct channel appear to be too high.
