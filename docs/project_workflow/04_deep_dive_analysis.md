# Deep Dive Analysis

## Introduction 

In the EDA process, having already established S (Stakeholder goals), C (Columns and coverage), and A (Aggregate and anomalies), the next step in the analysis involves **N (Notable segments)** grouping metrics by category, time, or other dimensions to uncover deeper insights.

## Deep Dive Analysis Framework

To avoid circular or aimless analysis, it is essential to establish a clear **North Star**.
The North Star defines the value required to achieve the objectives of the analysis, encompassing:
- Metrics
- Dimensions
- Team Goals

## Deep Dive Analysis Process

In this project:

North star metrics: USD_PRICE
  - Focus on the USD_PRICE column to derive Total Revenue. You may also look into Order Count and AOV. 
  - However, as there are no specific stakeholder requirements, the current focus will be on USD_PRICE and Total Revenue.

North star dimensions: REGION, MARKETING_CHANNEL, PRODUCT, TIME
  - Because stakeholders are not just looking for raw numbers; they want to see movement. Insights are gained by observing how dimensions change over time, rather than simply looking at their absolute magnitude.

North star team goals:
  - Marketing Team: How can we attract more customers or encourage them to increase their purchase volume? 
  - Product Team: Which products or features are the most popular? 
  - Finance Team: Where is the revenue—or loss—coming from?

We will use these North Star metrics to determine how to segment the data, identify which insights to prioritize, and formulate recommendations for each team.

## Deep Dive Insight 

The following are the findings obtained after conducting further analysis using Power BI.

| Graphic | Insight |
| --- | --- |
| Overall sales trend (overall_USD) | Sales more than doubled in early 2020, peaking in September and December 2020. However, sales declined significantly starting in January 2021. |
| Overall sales by product (product_USD) | The 27-inch 4K gaming monitor, Nintendo Switch, and Sony PlayStation 5 bundle are the primary drivers behind the decline in overall sales; all three exhibited a similar trend of plateauing in 2021. |
| Overall sales by marketing channel (marketing_USD) | Direct sales are the primary driver of high sales volume, while other marketing channels lag far behind. | 
| Overall sales by region (region_USD) | All regions showed a similar decline in sales in 2021, which indicates the presence of a global or macro-level trend. |
| Overall sales by product split by marketing channel | Although the three best-performing products experienced a decline in sales in early 2021, the Sony PlayStation 5 Bundle saw a particularly significant drop, driven primarily by a decline in direct sales that has continued downward. |
| Overall sales by product split by region | Sales of Sony PlayStation 5 bundles have seen their largest decline in North America via direct sales, which points to a shift in trends or increased competition in that region. |

## Determine Recommendation

To determine recommendations for each team, insights can be categorized into three different groups.

Stakeholder insights fall into three categories across all industries:
1. Contextual: Insights that are useful to know, but which we cannot influence.
2. Directional: Insights that point toward areas for further exploration; as such, it is not yet possible to draw definitive conclusions about the next steps.
3. Actionable: Insights that are clear and realistic enough for the team to act upon.
   These are further divided into two types:
  - Short-term: concrete matters with clear, tangible follow-up actions.
  - Strategic/long-term: insights that suggest a shift in direction.

#### A. High Level Sales

| Initial insight | Deep dive insight |
| --- | --- |
| Total sales from 2019 to 2022 amounted to approximately $6.1M, with monthly sales ranging from $80K to $500K. | Sales more than doubled in early 2020, peaking in September and December 2020. However, sales declined significantly starting in January 2021. |

Insight Category:
- Directional, The insight focuses solely on one metric without incorporating any dimensions; further investigation is required to understand the underlying business context.
- Contextual, It is worth noting that in early 2020, as COVID-19 cases surged and many people were sent home, individuals began spending more of their time at home including seeking out entertainment. This is why sales saw a dramatic increase during that period.

Recommendation:
1. Finance/Analytics Team
  (Directional) Investigate further the root causes of the decline in sales during the year COVID-19 occurred, including an analysis broken down by product and region.
2. General
  (Contextual) Given that people were spending more time at home, there was an increased demand for entertainment, which included the purchase of gaming products.

#### B. Product Insight

| Initial insight | Deep dive insight |
| --- | --- |
| - The product with the best sales performance is the 27-inch 4K gaming monitor, reaching $2M. <br> - The product with the worst sales performance is the Razer Pro Gaming Headset, with a total of $800K. <br> - It is necessary to check for missing values ​​in the sales data in coordination with the relevant team. |
| Gaming headset products (JBL Quantum 100 Gaming Headset & Razer Pro Gaming Headset) only contribute approximately 2% of total sales. | |
| A significant surge in sales occurred in December 2020. The Fall-Winter season, leading up to the new year, was recorded as the period with the best performance. | |

Insight Category:
- Actionable, findings that are immediately actionable because they relate directly to the product.

Recommendation:
1. Product Team
  Remove gaming headsets (JBL Quantum 100 Gaming Headset & Razer Pro Gaming Headset) from the inventory, as they account for only 2% of overall revenue.
2. Marketing Team:
  - Focus on promoting the 27-inch 4K gaming monitor, Nintendo Switch, and Lenovo Ideapad Gaming 3 in North America, as these items show strong market appeal. 
  - Strengthen promotional efforts for the winter season by pushing the top 4 products during October or November.
3. Data Team:
  - Investigate missing values ​​in the sales data, specifically within the `USD_PRICE` field. 
  - Check for missing values in the sales data.

#### C. Regional Insight

| Initial insight | Deep dive insight |
| --- | --- |
| - All product types experienced a significant increase in sales from 2020 onwards, following the overall sales trend. <br> - There was a macro-level or company-wide impact (initially presumed to be caused by COVID). | All regions showed a similar decline in sales in 2021, which indicates the presence of a global or macro-level trend. |
| Almost all products experienced a surge in sales in December 2020; it is worth examining the promotions or campaigns that took place during that period. | |

Insight Category:
- Contextual, It is impossible to influence an event that has become a global trend; however, it is much easier to analyze a rise in sales when it occurs in a specific region, as we can then identify what distinguishes that area from others.

#### D. Marketing Insight

| Initial insight | Deep dive insight |
| --- | --- |
| | Direct sales are the primary driver of high sales volume, while other marketing channels lag far behind. |

Category Insight:
- Directional, The figures require further investigation, as they do not align with established marketing domain knowledge.
- Actionable, Adjustments can be implemented immediately across marketing channels with known potential.

Recommendation:
1. Data Team
  Double-check that the attribution/data source for this marketing channel is correct. The direct channel figures appear to be too high.
2. Marketing Team
  Focus marketing strategies on the email channel, which shows potential for growth and could help reduce reliance on the "direct" channel.
  
