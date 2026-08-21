# Sales Performance Analysis

## Project Overview

This project presents an interactive Sales Analysis Dashboard built in Microsoft Power BI to analyze sales performance from 2019 to 2021. The dashboard provides an executive view of sales, profit, discounts, quantity, customer segments, regional performance, product sub-categories, sales trends and geographic distribution across the United States.

## Dashboard Objectives

The dashboard is designed to measure overall sales and profitability, identify the strongest customer segments and geographic markets, understand sales trends, rank product sub-categories, and provide an interactive executive reporting
experience.


## Key Performance Indicator

|KPI|Result|Interpretation|
|--------|--------|--------|
|Total|38k|Approximately 30,000 units sold|
|Discount|1.56k|Total discount value displayed|
|Profit|266.40k|Total Profit generated|
|Sales|2.30m|Total sales revenue|

The displayed figures imply an estimated profit margin of approximately 12.45% (286.40K ÷ 2.30M)


## Sales by Customer Segment

|Segment|Sales|Shares %|
|--------|--------|--------|
|Consumer|1.8m|50.55%|
|Corporate|0.7m|30.74%|
|Home Office|0.43m|18.70%|

Consumer customers are the largest revenue contributor, accounting for about half of sales. Corporate customers provide a significant secondary revenue stream, while Home Office represents a smaller share.

## Sales by Region

|Region|Sales|Shares %|
|--------|--------|--------|
|West|$725.46k|31.58%|
|East|$678.78k|29.55%|
|Central|$501.24k|21.83%|
|South|$391.46k|17.04%|

West is the strongest region at 31.58%, followed closely by East at 29.55%. Together they contribute roughly 61% of regional sales. South is the lowest contributor and may warrant a focused growth review.


## Sales Trend Analysis

The order-date chart shows substantial variation in sales from 2019 through 2021, including several pronounced spikes. Sales are not evenly distributed across the timeline. Recommended enhancements include year-over-year growth, monthly and quarterly totals, moving averages and seasonality analysis.


## Performance by Sub-Category

Phones appear to be the strongest-performing visible sub-category, followed by categories such as Chairs and Storage. Lower-ranking categories include Fasteners, Labels, Envelopes and Supplies. Sales should be evaluated alongside profit margin before inventory or product-prioritization decisions.


## Geographic Distribution

The map shows sales locations distributed across the United States. This view can support analysis of market penetration, underperforming states, distribution efficiency and expansion opportunities.


## Dashboard Interactivity & Design

The dashboard includes Country/Region and Category filters, KPI cards, donut charts, bar charts, a sales trend chart and a geographic map. It dark navy and gold executive theme provides strong visual hierarchy and consistent branding

 ## Key Business Findings
 
• Consumer customers dominate sales at approximately 50.55%.

• West is the strongest region at approximately 31.58%.

• West and East together contribute about 61% of regional sales.

• Phones are a leading visible product sub-category.

• Total sales are approximately $2.30M.

• Total profit is approximately $286.40K, implying an estimated 12.45% margin.


## Power BI Measures

- Total Sale
  
~~~Total Sales
=SUM(Sales[Sales])
~~~

- Total Profit
  
~~~Total Profit
=SUM(Sales[Profit])
~~~

- Total Quanty
  
~~~Total Quantity
=SUM(Sales[Quantity])
~~~

- Total Diacount
  
~~~Total Discount
=SUM(Sales[Discount])
~~~

- Profit Margin

~~~Profit Margin
=DIVIDE([Total Profit], [Total Sales], 0)
~~~

- Sales YOY

~~~Sales YoY
=CALCULATE([Total Sales], SAMEPERIODLASTYEAR(Sales[Order Date]))
~~~

- Sales YoY Growth
  
~~~Sales YoY Growth %
=DIVIDE([Total Sales] - [Sales YoY], [Sales YoY], 0)
~~~


## Recommendations

The main goal should be to increase profitable sales, not just revenue.

- Focus on high-performing products such as Phones, Chairs and Storage.

- Increase average order value through bundles, upselling and cross-selling.

- Reduce unnecessary discounts to protect profit margins.

- Target Corporate customers with larger office/product packages.

- Strengthen the West and East regions, which generate about 61% of regional sales.

- Investigate the South region to understand why it has the lowest sales share.

- Develop Home Office packages to grow its current ~19% contribution.

- Improve customer retention and encourage repeat purchases.

- Analyze sales spikes to identify successful products, regions and periods that can be replicated.

- Add Profit Margin, Average Order Value, Sales Growth and Repeat Customer Rate to the Power BI dashboard.

Bottom line: Focus on high-margin products + larger customer orders + less unnecessary discounting + stronger Corporate sales + targeted regional growth. This should help the business increase both sales and profit, rather than increasing sales while sacrificing margin.










