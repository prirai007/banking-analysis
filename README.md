Project Overview
This repository contains an analytics project for the banking domain, focusing on client and account-level insights. We perform exploratory data analysis (EDA) on sample banking data using a Jupyter Notebook with Pandas, extract and prepare data via MySQL, and build interactive business intelligence dashboards in Power BI. The goal is to surface key metrics such as total clients, total deposits, total loans, fees, and average account balances, along with breakdowns by income segment and nationality. EDA is the process of analyzing datasets to summarize their main characteristics, identify patterns, and detect anomalies


Features and Insights
Data Extraction & Preparation: Raw data is stored in MySQL tables. We use SQL queries to retrieve and aggregate this data, then load the results into Pandas DataFrames for analysis. This approach simplifies the analysis workflow by converting query results directly into data frames

Exploratory Data Analysis (EDA): Using Pandas in Jupyter Notebook, we examine distributions and trends (e.g., age, income, account balances). We clean the data (handling missing values and anomalies) and create visualizations (histograms, box plots, etc.) to uncover patterns and relationships.

Key Metrics (KPIs): We compute business-critical metrics such as Total Clients, Total Deposits, Total Loans, Total Fees Collected, and Average Account Balance. We also analyze ratios and segments (e.g., loan-to-deposit ratio, fee breakdown by type). For example, we highlight that “a bank with high deposits is considered reliable and trustworthy” when assessing financial health

Segmentation: Insights are broken down by client demographics. We segment clients by Income Brackets and Nationality to reveal which groups contribute most to deposits, loans, and other KPIs.

Power BI Dashboards: Interactive dashboards are built to display the analysis results. These dashboards consolidate multiple data sources on a single canvas, providing a holistic view of performance trends

Users can filter the dashboards by date ranges, client segments, or other categories to drill into specific KPIs.


Data Sources
Banking.csv: Core banking dataset with 3,000 records. Includes fields like Client ID, Age, Nationality, Estimated Income, deposit and loan amounts, account balances, fees, etc.
clients.csv: Lookup table for client attributes (e.g., mapping Gender ID to Gender).
Note: These tables simulate the types of data one would find in a bank’s database. They can be imported into MySQL or used directly as CSVs in the analysis.


Tools and Technologies Used
Python & Pandas: For data loading, cleaning, and EDA. Pandas allows efficient analysis of tabular data

MySQL: Relational database to store and query the raw data. We connect via Python (e.g. PyMySQL) to fetch query results into Pandas

Power BI: Used to design interactive dashboards and reports. Power BI enables creation of tailored visualizations and provides a holistic view of key metrics

Jupyter Notebook: Interactive environment for writing and executing the analysis code.
Matplotlib/Seaborn: Python libraries for data visualization (charts and plots).
Notebooks and Dashboard Files
banking_eda.ipynb – Jupyter Notebook containing the EDA workflow (data loading, cleaning, analysis, and visualizations).
mysql_queries.sql – SQL script(s) for extracting and aggregating data from the MySQL database.
banking_dashboard.pbix – Power BI report file with the interactive dashboards (e.g., overview and KPI pages).
(Add any other relevant files or resources here.)
How to Use the Project
Setup: Install Python (with Pandas, Matplotlib, PyMySQL, etc.) and MySQL. Also install Power BI Desktop to view the dashboards.
Prepare Data: Import the CSV files into the MySQL database or place them in a data/ folder. Run mysql_queries.sql in MySQL to set up any required tables or views.
Run the Notebook: Open banking_eda.ipynb in Jupyter. Update database connection parameters or file paths as needed. Execute all cells to perform the analysis and generate plots.
View Dashboards: Open banking_dashboard.pbix in Power BI Desktop. Refresh the data source if prompted. Use slicers and filters to explore metrics by time period, client segment, nationality, etc.
Note: This project is analytical only and is not deployed as an application or web service.

 A consolidated dashboard view helps bank executives see overall performance at a glance. The example below is a placeholder showing a Power BI financial dashboard layout that combines profit/loss KPIs with monthly trend charts. For instance, the top cards display KPI summaries (e.g. profit margin and revenue), while the plots show how income and expenses evolve over time.
 
 Power BI dashboards provide a holistic view of key metrics and performance indicators. The screenshot below (placeholder) includes KPI tiles and a funnel chart. In a banking scenario, similar visuals could represent customer acquisition funnels or account sign-up stages, with KPIs highlighting totals for clients, deposits, and loans.


