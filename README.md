# Customer Sales Analysis for Online Store

Table of Contents
- [Objectives](#objectives)
- [About the Data](#about-the-data)
- [Executive Summary](#executive-summary)
- [Data Cleaning and Exploration](#data-cleaning-and-exploration)
- [Data Analysis](#data-analysis)
- [Insights & Recommendations](#insights-&-recommendations)
- [Caveats](#caveats)

***

## Objectives
 - The company aims to evaluate its customer database and identify potential growth opportunities.
 - To boost sales and expand its customer base, the company plans to launch a new advertising campaign but is uncertain about the target audience or geographic focus.
  
## About the Data
This is an open-source dataset, obtained from Kaggle, and intended for training and practice purposes. The Excel Spreadsheet has 1027 rows and 13 columns. The column names are:  ID, Marital Status, Gender, Income, Children, Education, Occupation, Home Owners, Cars, Commute Distance, Region, Age, Purchases.
Click [here](https://github.com/aKotiAnalyst/Excel---Project/blob/main/Online%20Shop%20-%20Customers%20Dataset%20-%20Original.xlsx) for the original dataset.

## Executive Summary
With a thorough analysis, as described in the subsequent steps, it was determined that the typical customer profile consists of married, adult or middle-aged (both male or female), residing in North America and primarily working from home, but targeted ads on the Adolescent segment and Asian market should greatly expand the customer base.

## Data Cleaning and Exploration
Data cleaning is a fundamental step in any data analysis process, as it ensures the data is accurate, consistent, and ready for meaningful interpretation. Raw datasets often contain errors, inconsistencies, duplicates, or missing values that can compromise the reliability of analysis and lead to flawed insights. By addressing these issues, data cleaning improves the quality and integrity of the dataset, enabling more accurate and trustworthy results. In this section, we outline the data cleaning steps undertaken to prepare the dataset for analysis, ensuring it meets the standards necessary for robust and actionable conclusions.

First, I checked for duplicate rows by selecting the table, going to the Data tab, and using the "Remove Duplicates" function 26 entries were removed.
![Remove duplicates](https://github.com/aKotiAnalyst/Excel---Project/blob/main/Images/Remove%20duplicates.JPG)

To enhance readability, I updated the "Marital Status" column by replacing "M" with "Married" and "S" with "Single." The “Gender” column was also updated by converting "F" to "Female" and "M" to "Male." I made sure to use the “Match entire cell content” option to not modify the heather just the columns.
![Improve readability](https://github.com/aKotiAnalyst/Excel---Project/blob/main/Images/Improve%20readability.JPG)
![Improve readability](https://github.com/aKotiAnalyst/Excel---Project/blob/main/Images/Improve%20readability%202.JPG)

I formatted the "Income" column to improve its visualization in the upcoming charts by converting the data type to Currency and reducing the decimal places.

![Income Column](https://github.com/aKotiAnalyst/Excel---Project/blob/main/Images/Income%20table.JPG)

On the “Commute Distance” column changed “10+ Miles” to “More than 10 Miles” so that it follows alphanumeric order.
![Daily Commute](https://github.com/aKotiAnalyst/Excel---Project/blob/main/Images/Daily%20Commute1.jpg) ![Daily Commute](https://github.com/aKotiAnalyst/Excel---Project/blob/main/Images/Daily%20Commute2.jpg)

I created an “Age Group” column to study the demographics. The parameters for grouping were Adolescent (younger than 20 years), Adult (between 20 and 40), Middle-Aged (40 to 60) and Senior (60 plus). For this reason, I choose an IF statement with multiple logical conditions.
![Age Group Column](https://github.com/aKotiAnalyst/Excel---Project/blob/main/Images/Age%20Group%20IF%20formula.JPG)

## Data Analysis
The segment of this project focuses on extracting meaningful insights from the cleaned dataset to address the research objectives. I employed pivot tables to efficiently organize, summarize, and analyze the data, extracting key insights to inform decision-making. To complement this, I integrated pivot charts, providing clear and impactful visualizations that addressed critical business questions and aligned with the project's objectives. By interpreting these findings, we aim to provide actionable conclusions and support evidence-based decision-making. The following analysis builds on the foundation of the prepared dataset, ensuring that the results are both accurate and impactful.

I used a cluster column chart titled “Avg Income Per Customer” to examine sale patterns, comparing married vs single and male vs female customers. 
![]()
![]()

I created a pie chart for a clear and straightforward overview of the distribution of daily commute distances.
![]()

I utilized a line chart to analyze at the “Customer Age Group” a column was specifically created to enhance the analysis. This was done after the dataset was thoroughly prepared and cleaned in the previous stages.
![]()

I created a doughnut chart to visualize and analyze the distribution of sales across different regions, providing a clear and concise overview of regional performance.
![]()

I integrated various visual elements to create a comprehensive dashboard. To enhance interactivity, I added three slicers, allowing users to filter the data dynamically and explore insights with ease.
![]()

Click [here] to examine (https://github.com/aKotiAnalyst/Excel---Project/blob/main/Online%20Shop%20-%20Customers%20Dataset%20-%20Analysis%20Project.xlsx) the final Excel Dashboard.

## Insights & Recommendations
 - The typical customer profile consists of married, adult or middle-aged (both male or female), residing in North America and primarily working from home.
 - The European market, accounting for only 23%, and the Pacific market, at 26%, are currently undervalued and present significant growth potential. Meanwhile, the Asian market, with 0% representation, offers a critical and untapped opportunity for expansion.
 - The Adolescent age group of the market offers substantial opportunities for growth and success, as it has been completely neglected and remains an untapped demographic. By strategically targeting this segment based on specific products, the company can unlock considerable potential and establish a strong presence in this overlooked area.

## Caveats
This analysis can be further refined by focusing on individual product sales instead of solely examining aggregate total sales. Such a detailed approach offers deeper insights into the performance of each product and enables the development of more targeted and effective strategies.







