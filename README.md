# Analyzing Social Media Marketing Campaign Performance: A Business Intelligence Approach Using Power BI, PostgreSQL and Python.

*How can marketing campaign data be leveraged to optimize ad performance, reduce costs, and improve conversion rates across channels and devices?*

## Introduction
Businesses continually rely heavily on online marketing campaigns to reach their target audiences, build brand awareness, and drive sales. With multiple channels available, including social media platforms like Facebook, Instagram, and Pinterest, it has become essential for marketing teams to track and analyze their advertising efforts to ensure optimal performance. 

This project focuses on analyzing a marketing campaign dataset to uncover patterns and insights that can help optimize ad performance. We'll be examining key metrics such as impressions, click-through rates (CTR), cost-per-click (CPC), conversions, and engagement metrics (likes, shares, comments), to provide a detailed overview of how different campaign ads perform across various channels, devices, and locations.

The analysis is conducted using Power BI, a powerful business intelligence tool that allows for data modeling, visualization, and reporting. Through this project, we seek to extract actionable insights that can lead to more informed decision-making, budget optimization, and improved ad targeting. 

The following sections will detail the problem questions, analytical approach, and insights generated from the data, along with recommendations for enhancing future marketing efforts.

## Problem Statement: 
This project aims to analyze marketing campaign data across different platforms, devices, and cities to uncover insights that inform data-driven decisions. Specifically, we want to identify trends in ad performance, assess cost efficiency, and determine which campaigns yield the highest conversions and engagement (likes, shares, comments).

## Business Questions
* Which channels (e.g., Facebook, Instagram, Pinterest) generate the highest number of impressions, clicks, and conversions?
* What is the top-performing location for each campaign in terms of conversions and total conversion value?
* How does device usage (mobile vs. desktop) impact the effectiveness of ad campaigns in terms of CTR, CPC, and conversions?
* How do the daily average CPC and ad spend correlate with conversions and conversion value?
* Which ad type leads to the highest engagement (likes, shares, and comments)?
* Are there any seasonal trends or patterns in campaign performance that can help with future campaign planning?

## Data Source
The dataset was obtained from the Onyx Data DNA Challenge for August. The data has 9900 rows and 18 columns. 

Python was used to connect, create and load the dataset into a PostgreSQL database. Sqlalchemy was used to achieve this. Thereafter, using power query, a connection to the database was established in order to extract the marketing data and transform it before loading it into Power BI for further analysis. 

Columns and their descriptions are outlined below.


# Skills Demonstrated

* Extract, Transform and Load (ETL) data using Python, SQL and PowerQuery

* Data Modeling in Power BI: 
Created a model linking performance metrics (e.g., impressions, clicks, spend, conversions) with ad campaigns, channels, cities, and devices.

* Data Visualization: 
Built interactive dashboards to visualize the relationships between ad performance metrics and different attributes such as channel, device, and location.

* DAX Calculations: 
Used DAX formulas to create custom measures, such as the total conversion value, CTR, and cost-per-click trends across campaigns.

* Insights Generation:
Derived actionable insights from the analysis, identifying areas where ad performance can be improved by reallocating ad spend or adjusting target locations and devices.

* Business Intelligence Reporting: 
Prepared a comprehensive Power BI report, summarizing campaign effectiveness, ad engagement, and recommendations for optimizing future marketing efforts.

## Data Pre-processing and Understanding
### Data Cleaning:

* Handle Missing Values: There were no missing values in the data.

* Remove Duplicates: No duplicate rows were found in the dataset.

* Format Data: Cost Per Click (CPC), Spend, and Conversion Value were formatted from numeric to currency format.

### Data Transformation:
* Calculated columns - Conversion rate, engagement rate, and return on Ad spend were created.
* A date table was created to use time intelligence functions.
### Data Modeling:
* Create Relationships: A one-to-many relationship was created between the data table and the marketing data.

* Create Measures: A measures table was created to store all the measures in one place. The image below shows the measures created for this analysis.



## Exploratory Data Analysis & Visualization
The analysis was structured based on the KPIs Engagement Rate, Conversion Rate, and Return on Ad Spend (ROAS) for the campaign preiod. To answer the business questions, it’s important to first explore and understand the data. 

* The data has 9900 rows and 18 columns.
* There are 3 campaign types (Fall, Summer and Spring)
* There are 3 locations (Birmingham, Manchester and London)
* The campaign channels are (Facebook, Instagram and Pinterest)
* The device types are (Desktop and Mobile)
* The campaigns consists of two Ad types (Collection and Discount)

## What are the Key Insights from the Analysis?

![overview](/JPEGS/overview.jpg)

### Campaign

* Despite campaigns in Fall having the highest Click-Through Rate, 1.35%, Summer had the highest 7.23% Engagement Rate and Fall recorded the lowest Engagement Rate.

* Campaigns in Summer had the highest Conversion Rate 32.85% and Fall recorded the lowest Conversion Rate 17.49% - despite having the highest CTR. 

* Return on Ad Spend was highest in Summer campaigns with July recording the highest ROAS. 

### Channel
* Instagram recorded the highest Engagement Rate 5.97% while Pinterest had the lowest Engagement Rate by a thin margin 5.14%.

* Pinterest had the highest Conversion Rate, 26.81% while facebook 18.97% had the lowest Conversion Rate.

* Pinterest had the highest Return on Ad Spend 2147.3% while facebook had the lowest 475.63% Return on Ad Spend.

### Ad and Device
* Campaigns with discount Ads had the highest Engagement Rate 6.82%. In terms of device type, desktop had the most Engagement Rate 6.32% as opposed to the Moblie devices with 4.89% Engagement Rate. 

* Campaings with discount Ads had the highest Conversion Rate 28.01% With desktop devices also having the highest 23.9% Conversion Rate. 

* Discount Ads had the highest Return on Ad Spend 57.09% compared to 42.91% for Collection Ads.\

* Desktop also recorded higher Return on Ad Spend 52.25%, while Mobile device had 47.75%

### Location
* Birmingham had the highest Engagement rate, 5.97%, while London had the lowest of the campaign Locations 5.02%.

* In terms of Conversion, Birmingham also had the highest Conversion Rate, 28.79% while London had the lowest 17.61%.

* Birmingham also had the highest Return on Ad Spend 1293% compared to London with the lowest Return on Ad Spend 697.8%.

### Data Visualization

![Engagement](/JPEGS/Engagement.jpg)

![Conversion](/JPEGS/Conversion.jpg)


![returns](/JPEGS/Return.jpg)




## Conclusion
The analysis of the marketing campaign data reveals several key insights:

* Summer campaigns were the most effective in terms of engagement and conversion rates.
* Instagram proved to be the most engaging platform, while Pinterest demonstrated the highest conversion rates and return on ad spend.
* Birmingham emerged as the top-performing location, surpassing London in terms of engagement, conversion, and return on ad spend.

## Recommendation
Based on these insights, the following recommendations can be made to optimize future marketing campaigns:

#### Focus on Summer Campaigns:
* Allocate more budget and resources to Summer campaigns, leveraging the high Engagement and Conversion Rates to maximize returns.
* Investigate and replicate elements of successful Summer campaigns for use in other seasons, particularly in Fall.
#### Optimize Channel Strategies:
* Continue leveraging Instagram for engagement-focused campaigns.
* Prioritize Pinterest for campaigns aimed at driving conversions and maximizing ROAS.
* Evaluate and refine Facebook strategies to improve performance or reallocate resources to better-performing channels.
#### Leverage Location Insights:
* Focus efforts on Birmingham, which shows consistently high engagement, conversion, and returns.
* Tailor campaigns specifically for underperforming locations like London, using localized strategies to address audience preferences and behavior.
#### Experiment with Seasonal Adjustments:
* Explore targeted promotions or unique creative strategies in Fall to improve its historically low engagement and conversion metrics despite its strong CTR.


## Appendix



