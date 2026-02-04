# Project Title: Designing a Sales Dashboard in Excel
### Submitted By: Prerna M. Kalambe

## 1. Objective 
<br>The objective of this project is to design a fully functional Sales Dashboard in Excel that allows users to:
<br> - •	Analyse sales based on different product categories
<br> - •	View month-wise sales and profit trends
<br> - •	Evaluate region-wise sales performance
<br> - •	Interact with the dashboard using a dynamic Combo Box
<br>
2. Dataset Description
The dataset provided contains detailed sales records with the following variables:
•	Order ID: Unique identifier for orders
•	Order Date / Ship Date
•	Product Category
•	Product
•	Sales, Quantity, Profit, Discount
•	Region, Country, City
•	Months (derived column)
•	Shipping Cost, Order Priority, Aging
This dataset was used to summarize monthly and regional performance.

3. Steps Performed
Step 1: Using the E-commerce dataset
Loaded the given sample dataset (“Sales Data” sheet) as instructed.
Step 2: Preparing the Working Sheet
A “Working” sheet was created to store backend calculations:
Created the following helper tables:
•	Month List (Jan–Dec)
•	Region List
•	Product Category List
•	Histogram Bins (if required)
Added column headers:
•	Month, Sales, Profit
•	Region, Region-wise Sales
Step 3: Created Month-wise Sales & Profit Table
Applied SUMIFS formulas to compute dynamic values based on category selection.
Sales:
=SUMIFS('Sales Data'!H:H, 'Sales Data'!U:U, $A4, 'Sales Data'!F:F, $R$3)
Profit:
=SUMIFS('Sales Data'!K:K, 'Sales Data'!U:U, $A4, 'Sales Data'!F:F, $R$3)
Step 4: Created Region-wise Sales Table
Computed region-wise totals using:
=SUMIFS('Sales Data'!H:H, 'Sales Data'!T:T, $F4, 'Sales Data'!F:F, $R$3)
Step 5: Created Combo Box (User Control)
A Combo Box was added to the Dashboard sheet:
•	Input Range: Working!Q2:Q5
•	Cell Link: Working!R2
Converted cell link index to actual selected category:
=INDEX(Working!Q2:Q5, Working!R2)
This enabled dynamic filtering of month-wise and region-wise values.
Step 6: Created Charts
Two main visuals were created:
1. Month-wise Sales vs Profit Chart (Column Chart)
Data source: A3:D15 (Month, Sales, Profit)
2. Region-wise Sales Chart
Data source: F3:G16 (Region, Sales)
Charts automatically refresh based on Combo Box selection.
Step 7: Designed the Dashboard
The dashboard layout includes:
•	Title: Sales Dashboard by Product Category
•	Combo Box for selecting product category
•	Month-wise trend chart
•	Region-wise sales chart
•	Section headers for clarity
The design was formatted professionally using consistent fonts, colors, and spacing.
8. Project Outcome
A dynamic Excel dashboard that:
•	Filters data by selected product category
•	Displays month-wise sales and profits
•	Shows region-wise sales distribution
•	Helps users easily analyze performance trends
All project requirements were successfully met.
9. Tools Used
•	Microsoft Excel
•	SUMIFS
•	Data Validation
•	Form Controls (Combo Box)
•	Charts (Column, Clustered Column)
•	Formatting and Layout Design


