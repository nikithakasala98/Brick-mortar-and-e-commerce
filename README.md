# Business Insights 360

## Project Overview

AtliQ Hardware has experienced significant growth in recent years. To maintain a competitive edge and make data-driven decisions, the company decided to implement data analytics using Power BI. This project aims to provide stakeholders with insights into various business aspects, including finance, sales, marketing, supply chain, and executive operations.

This project was developed following the Codebasics Power BI Course. You can find the course [here](https://codebasics.io/courses/power-bi-data-analysis-with-end-to-end-project)

[Live Report Link](https://app.powerbi.com/view?r=eyJrIjoiOTViNjIwYjUtZDBhOS00MzFjLWI4NDItODU2NjFiZTY2MDQzIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&pageName=ReportSection0e765c0061580b067c73)

## Tech stacks

- SQL
- PowerBI Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)
- Project charter file

## Power BI Techniques Acquired

-	Creating Calculated Columns
-	Crafting Measures using DAX Language
-	Data Transformation
-	Data Modeling
-	Data Validation Techniques
-	New Card visual
-	DAX formulas for Color change of visuals
-	Utilizing Bookmarks for Visual Switching
-	Page Navigation with Buttons
-	Using the divide function to prevent zero division errors
-	Building Date Tables with M Language
-	Dynamic Titles based on Filters
-	KPI Indicators
-	Conditional Formatting in Visuals
-	Power BI Services
-	Publishing Reports to Power BI Services
-	Setting up Personal Gateway for Auto-refresh

## GitHub 

- Uploading Large size files using GitHub LFS
- Tracking the particular type of file extensions for LFS

## Business Terminology Learned

- Gross price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice sale
- Gross Margin
- Net sales
- Net profit
- COGS - cost of goods sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer
- Benchmark Values
- Revenue Contribution
- Excess Inventory
- Unit Economics

## Soft Skills acquired during Project development:
- Analytical Thinking: Identifying patterns and insights from complex data.
- Problem-solving: Overcoming challenges in data modeling and visualization.
- Communication: Conveying data-driven stories effectively to stakeholders.
- Attention to Detail: Ensuring accuracy and precision in reports.
- Time Management: Balancing multiple tasks and meeting deadlines.

## Company’s background

AtliQ Hardware is a rapidly growing company with a global presence, specializing in computers and computer accessories sold through three channels:

- Retailers
- Direct Sales
- Distributors

Recently, the company faced unexpected losses after opening a store in America, relying on surveys, intuition, and limited Excel analysis. Meanwhile, competitors have robust analytics teams that drive data-driven decisions. To remain competitive, AtliQ Hardware has prioritized building its analytics team to gain data-driven insights for better decision-making. 

## Project kick-off
Before starting the project, it’s crucial to have a clear understanding of the objectives and expectations. Consider the following questions:

- What is the objective of building this Power BI dashboard?
- How will the success of this project be measured?
- What is the project deadline?
- Do stakeholders expect a preview before the final release?
- What are the stakeholders' expectations and concerns?
- Who will use this dashboard, and for what purpose?
- What are the stakeholders' expectations upon project completion?
- What potential challenges could arise during the project?
- What resources and data are needed to build this dashboard?
- Are there any specific inputs from stakeholders regarding the design     and layout of the dashboard?
- 
Following the project kick-off meetings, the data engineering team will provide the necessary data. The next step is to explore the dataset.

### Dataset **Understanding.**

Understanding the available data is crucial before beginning the analysis. The dataset is divided into:

Dimension Tables: Contain static data such as customer and product details.

Fact Tables: Contain transactional data.  

- gdb041:
    - `dim_customer`
        - **27** distinct markets (ex India, USA, Spain)
        - **75** distinct customers across markets
        - **2** platform types:
            - Brick & Motors(Physical stores)
            - E-commerce(Online stores like Amazon, Flipkart)
        - 3 channels: Retailer, Direct, Distributors
    - `dim_market`
        - **27** distinct markets (ex India, USA, Spain)
        - 7 sub-zones
        - 4 regions
            - APAC
            - EU
            - nan
            - LATAM
    - `dim_product`
        - Divisions
            - P & A
                - Peripherals
                - Accessories
            - PC
                - Notebook
                - Desktop
            - N & S
                - Networking
                - Storage
        - 14 different categories (e.g., Internal HDD, keyboard)
        - Various product variants available
    - `fact_forecast_monthly`
        - Used for forecasting customer needs to enhance customer satisfaction and reduce storage costs.
        -The table is denormalized, and optimized for analytical work.
        -All dates are replaced by the start date of the month.
        -The table ends with the forecast quantity needed by the customer.
    - `fact_sales_monthly`
        - Similar to the fact_forecast_monthly table, but with sold quantity instead of forecast quantity.
- gdb056:
    - `freight_cost`
        - Details of travel and other costs for each market by fiscal year.
    - `gross_price`
        - Gross prices with product codes.
    - `manufacturing_cost`
        - Manufacturing costs with product codes by year.
    - `Pre_invoice_dedutions`
        - Pre-invoice deductions percentage for each customer by year.
    - `Post_invoice_deductions`
        - Post-invoice deductions and other deduction details.

## Importing Data into PowerBI

- The dataset is stored in a MySQL database. To import the data into Power BI, provide the necessary database access credentials.

## Data Model

- Data modeling is critical and serves as the foundation of the report. The visuals are built upon the data model.
- Poor data modeling can negatively impact the report's performance.
- Follow best practices for data modeling. Refer to this blog for more information. [Blog](https://addendanalytics.com/blog/data-modelling-best-practices/)
- This project follows the Snowflake data modeling method.

<img src="https://github.com/Naveen-S6/Business_Insights_360/blob/main/Resources/Data_model.png" class="center">

### Dashboard designing

Based on the received mock-ups, the team will start designing the visuals and creating measures as needed.

## Home view

The Home View contains buttons that lead to different sections of the report. Users can navigate to specific pages by clicking the buttons:

- Info
- Finance View
- Sales View
- Marketing View
- Supply chain View
- Executive View
- Filter
- Support

## Home Report

![Home Report](https://github.com/nikithakasala98/Brick-mortar-and-e-commerce/blob/main/Resources/Home.gif)

## Info Page

![Info](https://github.com/nikithakasala98/Brick-mortar-and-e-commerce/blob/main/Resources/information.gif)

## Finance View

![Finace](https://github.com/nikithakasala98/Brick-mortar-and-e-commerce/blob/main/Resources/Finance.gif)

## Sales View

![Sales](https://github.com/nikithakasala98/Brick-mortar-and-e-commerce/blob/main/Resources/Sales.gif)

## Marketing View

![Marketing](https://github.com/nikithakasala98/Brick-mortar-and-e-commerce/blob/main/Resources/Market.gif)

## Supply chain View

![Supply chain](https://github.com/nikithakasala98/Brick-mortar-and-e-commerce/blob/main/Resources/Supply-Chain.gif)

## Executive View

![Executive](https://github.com/nikithakasala98/Brick-mortar-and-e-commerce/blob/main/Resources/Executive.gif)


you can find the full report file here : [Report](https://github.com/nikithakasala98/Brick-mortar-and-e-commerce/blob/main/Report/Data_Analysis_360degrees_Project.pbix)


## Project Outcome

This report enables data-driven decision-making and provides answers to a variety of "why" questions based on the situation.
