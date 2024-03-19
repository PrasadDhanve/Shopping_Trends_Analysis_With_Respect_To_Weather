# Shopping Trends Analysis Of Istanbul City With Respect To Weather
![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/8e63e46e-4bdb-4c16-b049-8feb139e7e86)

## Introduction

This project presents an analysis of shopping trends based on weather conditions using two datasets: Istanbul sales data from 2021 to 2023 and Istanbul weather data from the same period. The analysis includes data preparation, exploratory data analysis (EDA), visualization, and insights derived from the data.

## Data Sources

- **Istanbul Sales Data (2021-2023):** Contains information about sales transactions in Istanbul, including date, product details, quantity sold, and revenue generated.
- **Istanbul Weather Data (2021-2023):** Includes weather data for Istanbul, such as temperature, humidity, wind speed, and weather conditions. Extracted from "https://www.visualcrossing.com/"

## Data Preparation

### Istanbul Sales Data

##### Business Problem
- Assuming that all the data is real and purchased from all shopping malls across Istanbul.
- The organization is asking for specific reports and presentations.
- For example, monthly income, annual income, sales amount in a certain age range, sales amount of categories, etc.
- They have asked us to share anything meaningful that we find during this process.
- Derive some patterns of shopping trends based on weather as well

![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/faa4b1ba-223e-47e9-9779-1b3435df6322)

##### Data Exploration Findings and Data Cleaning
- The data type of the "Date" column was incorrect.
- There were no null values present.
- Duplicated rows were not found in the dataset.
- There were no instances of repeated strings representing the same class in any columns.
- The "Invoice" and "Customer ID" columns were unnecessary as there were no repeated invoices or customers; every value was distinct, and we already had the index.
- Columns for day, weekday, month, and year were added to identify trends based on the timeframe.
- Ages were categorized into different groups to analyze the shopping trends of each age group.

##### Functions
- The 'value_counts' function takes a data frame as input and returns the value counts of all the columns.
- The 'bar_plot' function uses Plotly Express to generate a bar chart displaying average spending per product for each category based on specified columns.
- The 'analyze' function groups the desired colums and perfrom aggregate function on 'quantity' and 'price' column.
- The 'pivot_bar' function creates the pivot table by grouping specified cols and performing agg as count on the value col.
- The 'line_chart' function groups the desired column and perfrom aggregate function on the 'quantity' and 'price' column.

![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/118841b0-07e6-4398-b891-72f94b4c1e7f)

![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/c6451d6c-4824-44ad-8d6a-4293bed3283c)

![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/8d4ea542-f991-4cd0-aa89-cd52a0b0dd4c)

##### Analysis And Visuallisation
- Performed analysis on the basis of gender.
- Analysis on the basis of categories as per gender
- Quantity Purchased by Gender
- Shopping distribution according to age.
- Finding which age cat generated more revenue.
- Payment Method Analysis.
- Analyzing Data By Timrframe(Y, M, W, D).

![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/3f3dc8bd-85bf-48f7-b533-26cfebf43c10)
![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/820c9f00-b527-43a5-a6e7-c9867cfa9061)
![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/0c7ad33a-481e-40b3-bc7e-94d985a33e65)

### Istanbul Weather Data

##### Business Problem
- The organization aims to analyze the impact of weather conditions on shopping trends in Istanbul.
- Specific reports and insights are required, such as correlation between weather elements and sales, seasonal trends, and weather-based shopping behavior.
- The organization is interested in any significant patterns or insights derived from the weather data analysis.

![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/3f3dd155-ec74-4e47-8010-5c4f184bbd92)

##### Data Exploration Findings and Data Cleaning
- Examined weather data from 2021 to 2023.
- The datetime column was not in the proper format.
- The 'precip_type' and 'icon' columns had many null values. We either dropped the columns or replaced the null values with 'unknown'.
- There were no duplicated records in the dataset.
- The categories in the dataset were unique, and there were no repeated strings or incorrect categories present.
- Categorized temperature into different ranges to analyze its impact on shopping trends.

##### Analysis And Visualization
- Analyzed the correlation between temperature, precipitation, and sales data.
- Visualized seasonal trends in weather and shopping behavior.
- Identified any significant patterns or anomalies in shopping trends based on weather conditions.
- Conducted trend analysis based on weather categories to understand customer behavior.

![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/ac6e97bb-8e20-4865-acc9-b822cf67b628)
![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/6cc60bd4-06ff-4cb7-a38f-57aacfe06090)
![image](https://github.com/PrasadDhanve/Shopping_Trends_Analysis_With_Respect_To_Weather/assets/148265382/93350d0f-cb98-4a3e-becb-7308ca58069e)

## Istanbul Shopping and Weather Analysis Dashboard.

### Overview
This dashboard analyzes the impact of weather conditions on shopping trends in Istanbul from 2021 to 2023. It explores temperature variations, weather patterns, product sales by category, and gender demographics.

### Insights

##### Temperature and Total Sales Comparison
Line chart showing sales trends based on temperature changes.
##### Products Sold by Categories and Gender
Stacked bar chart depicting product sales by category and gender.
##### Temperature Categories
Heat map categorizing temperature conditions.
##### Weather Type Across Months
Bar chart illustrating weather distribution across months.

### Key Findings
- Moderate temperatures correlate with higher sales.
- Popular categories differ by gender.
- Stable weather conditions are predominant.
- Rainy weather impacts shopping behaviors.
- This analysis helps businesses understand how weather influences consumer behavior, aiding in strategic decision-making and optimization.

## Conclusion
The Istanbul Shopping and Weather Analysis project provides valuable insights into the impact of weather conditions on shopping trends in Istanbul from 2021 to 2023. Through data preparation, exploration, and visualization of Istanbul sales and weather data, several key findings have emerged. Understanding the interplay between weather conditions and consumer behavior is crucial for businesses to make informed decisions. By leveraging insights from this analysis, organizations can optimize marketing strategies, inventory management, and promotional activities to capitalize on favorable weather conditions and mitigate risks during adverse weather events.
