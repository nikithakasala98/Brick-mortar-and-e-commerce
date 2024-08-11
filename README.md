# Business Insights 360

## Project Overview

AtliQ Hardware has been proliferating in recent years, and they have decided to implement data analytics using PowerBI in their company for the first time to surpass their competitors in the market and to make data-driven decisions. This project hopes to give answers to the questions of stakeholders in terms of all aspects like finance, sales, marketing, supply chain and executive.

I worked on this project by following the Codebasics PowerBi Course, Link to the course is [here](https://codebasics.io/courses/power-bi-data-analysis-with-end-to-end-project)

[Live Report Link](https://app.powerbi.com/view?r=eyJrIjoiOTViNjIwYjUtZDBhOS00MzFjLWI4NDItODU2NjFiZTY2MDQzIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&pageName=ReportSection0e765c0061580b067c73)

## Tech stacks

- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)
- Project charter file

## PowerBI techniques Learnt

- What are all the questions that should be asked before starting the project
- Creating calculated columns
- creating measures using the DAX language
- Data modeling
- Using Bookmarks to switch between two visuals
- Page navigation with buttons
- Using the divide function to prevent zero division errors
- creating data table using m language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting of the values in visuals using icons or background colour
- Data validation techniques
- PowerBi services
- Publishing reports to PowerBi services
- Setting up the personal gateway to set up the auto-refresh of data
- PowerBi App creation
- Collaboration, workspace, and access permissions in PowerBI services
- And more 😅

## GitHub 

- Uploading Large size files using GitHub LFS
- Tracking the particular type of file extensions for LFS

## Business related terms

- Gross price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice sale
- Gross Margin
- Net sales
- Net profit
- COGC - cost of goods sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer

## Company’s background

AltiQ Hardware is a company which has grown vastly in recent years, and opened business all over the globe. It is a company which sells, computers and computer accessories through three mediums/channel

- Retailers
- Direct
- Distributors

Recently the company has faced an unforeseen loss by opening a store in America based on the surveys, intuition and some Excel analysis also the company’s competitors have a handful of analytics teams to perform analysis and make data-driven decisions. So, The AltiQ hardware has no option other than building its analytics team for data-driven insights and decisions in the future to survive better in the industry. 

Project kick-off session, where you should get clear of what and why this project is and all other questions you have with regards to the project

### Questions to ask before starting with the dashboard

- What is the objective of building this PowerBi dashboard?
- On what terms the success of this project measured?
- What will be the deadline of the project?
- Do the stakeholders expect a preview before the actual release?
- What are the hopes of the stakeholders out of this project?
- What are the fears stakeholders have in terms of building this dashboard?
- Who will be using this dashboard and for what purpose?
- What are the expectations of stakeholders by the completion of this project?
- What can go wrong while building this project?
- What are all the resources/ data needed to build this dashboard?
- Is there any input from stakeholders in terms of design and views of the dashboard?

After the project kick-off meetings, the data engineering team has given the data as per the request of the data analytics team, let’s explore them.

### Dataset **Understanding.**

Understanding what data is available will be more helpful while doing analysis. Before jumping on to the analysis get the provided data analysed.

Dimension table: Has static data like details of customers and products

Fact table: Has the data of the transactions  

- gdb041:
    - dim_customer
        - **27** distinct markets (ex India, USA, Spain)
        - **75** distinct customers throughout the market
        - **2** types of platforms
            - Brick & Motors - Physical/offline store
            - E-commerce - Online Store (Amazon, Flipkart)
        - Three channels
            - Retailer
            - Direct
            - Distributors
    - dim_market
        - **27** distinct markets (ex India, USA, Spain)
        - 7 sub-zones
        - 4 regions
            - APAC
            - EU
            - nan
            - LATAM
    - dim_product
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
        - There are 14 different categories, Like Internal HDD, keyboard
        - There are different variants available for the same product
    - fact_forecast_monthly
        - This table is used to forecast the customer’s needs in advance, which can help in
            - Higher customer satisfaction
            - Reduced cost in warehouses for storage purposes
        - The data engineering team denormalizes the table. It is a data warehouse that aims to be used for analytical work.
        - All the dates of the month should be replaced by the start date of the month
        - It has all the column names and in the end, it has the forecast quantity needed by the customer
    - fact_sales_monthly
        - This table is more or less is same as the fact_forecase_monthly table, but the last column has the value of the sold quantity instead of the forecast value.
- gdb056
    - freight_cost
        - This table has details of travel costs and other costs for each market with fiscal year.
    - gross_price
        - Having details of gross prices with product codes.
    - manufacturing_cost
        - Having details of manufacturing cost with product code with year.
    - Pre_invoice_dedutions
        - Having the details of pre-invoice deductions percentage for each customer with year
    - Post_invoice_deductions
        - Post invoice deductions and other deduction details

## Importing data into PowerBi

- As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBI by providing the Database access credential

## Data Model

- Data modeling plays a vital role and is considered the report's basement. All the visuals will be built upon the data model.
- Poor data modeling affects the overall performance of the report.
- Following Good practices of data modeling is a must. Refer to this page to get to know the good practices [Blog](https://addendanalytics.com/blog/data-modelling-best-practices/)
- In this project, we have followed the Snowfall data modeling method.

<img src="https://github.com/Naveen-S6/Business_Insights_360/blob/main/Resources/Data_model.png" class="center">

### Dashboard designing

Based on the mock-ups received as a requirement, the team will start designing the visuals and create measures as and when required

## Home view

In-Home view, all the views button will be available. Users will land on a specific view page by clicking the button 

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

![Info](https://github.com/nikithakasala98/Brick-mortar-and-e-commerce/blob/main/Resources/BI-360_Info.mp4)

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

By using this report, decisions can be made based on the data. Further, it will help answer ##n number of why questions based on the situation.
