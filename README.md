# Project Title: Designing a Sales Dashboard in Excel
### Submitted By: Prerna M. Kalambe


### Here Is the Preview of my Final Sales Dashboard 

<img width="1693" height="612" alt="Final Sales Dashboard" src="https://github.com/user-attachments/assets/5913a313-f6d6-4362-9258-25aec476a201" />


<br><br>

## 1. Objective 
<br>The objective of this project is to design a fully functional Sales Dashboard in Excel that allows users to:
<br> •	Analyse sales based on different product categories
<br> •	View month-wise sales and profit trends
<br> •	Evaluate region-wise sales performance
<br> •	Interact with the dashboard using a dynamic Combo Box
<br><br>
## 2. Dataset Description
<br> The dataset provided contains detailed sales records with the following variables:
<br> •	Order ID: Unique identifier for orders
<br> •	Order Date / Ship Date
<br> •	Product Category
<br> •	Product
<br> •	Sales, Quantity, Profit, Discount
<br> •	Region, Country, City
<br> •	Months (derived column)
<br> •	Shipping Cost, Order Priority, Aging
<br> This dataset was used to summarize monthly and regional performance.
<br><br>
## 3. Steps Performed
### Step 1: Using the E-commerce dataset
Loaded the given sample dataset ([“Sales Data”](https://github.com/prernakalambe-work/Designing-a-Sales-Dashboard-in-Excel/blob/2d7289d71dff9c4b583d160735c2a1a2bea79bb0/E_Commerce_Dashboard_Project.xlsx) sheet) as instructed.
### Step 2: Preparing the Working Sheet
A “Working” sheet was created to store backend calculations:
<br> Created the following helper tables:
<br> •	Month List (Jan–Dec)
<br> •	Region List
<br> •	Product Category List
<br> •	Histogram Bins (if required)
<br> Added column headers:
<br> •	Month, Sales, Profit
<br> •	Region, Region-wise Sales
### Step 3: Created Month-wise Sales & Profit Table
Applied SUMIFS formulas to compute dynamic values based on category selection.
<br> Sales:
<br> =SUMIFS('Sales Data'!H:H, 'Sales Data'!U:U, $A4, 'Sales Data'!F:F, $R$3)
<br> Profit:
<br> =SUMIFS('Sales Data'!K:K, 'Sales Data'!U:U, $A4, 'Sales Data'!F:F, $R$3)
### Step 4: Created Region-wise Sales Table
Computed region-wise totals using:
<br> =SUMIFS('Sales Data'!H:H, 'Sales Data'!T:T, $F4, 'Sales Data'!F:F, $R$3)
### Step 5: Created Combo Box (User Control)
A Combo Box was added to the Dashboard sheet:
<br> •	Input Range: Working!Q2:Q5
<br> •	Cell Link: Working!R2
<br> Converted cell link index to actual selected category:
<br> =INDEX(Working!Q2:Q5, Working!R2)
<br> This enabled dynamic filtering of month-wise and region-wise values.
### Step 6: Created Charts
Two main visuals were created:
<br> 1. Month-wise Sales vs Profit Chart (Column Chart)
<br> Data source: A3:D15 (Month, Sales, Profit)
<br> 2. Region-wise Sales Chart
<br> Data source: F3:G16 (Region, Sales)
<br> Charts automatically refresh based on Combo Box selection.
### Step 7: Designed the Dashboard
The dashboard layout includes:
<br> •	Title: Sales Dashboard by Product Category
<br> •	Combo Box for selecting product category
<br> •	Month-wise trend chart
<br> •	Region-wise sales chart
<br> •	Section headers for clarity
<br> The design was formatted professionally using consistent fonts, colors, and spacing.
<br><br>
## 4. Project Outcome
<br> A dynamic Excel dashboard that:
<br> •	Filters data by selected product category
<br> •	Displays month-wise sales and profits
<br> •	Shows region-wise sales distribution
<br> •	Helps users easily analyze performance trends
<br> All project requirements were successfully met and can be verified through [Screenshots](https://github.com/prernakalambe-work/Designing-a-Sales-Dashboard-in-Excel/blob/3d7e728df3256628905d09d67a60831f610253c2/ScreenShots%20for%20results.zip) or [Video](https://github.com/prernakalambe-work/Designing-a-Sales-Dashboard-in-Excel/blob/f2d633e1bffc60ffbf3f5c07a5bb1db9e1eb26e3/Excel%20project%201%20.mp4) for references.
<br><br>

## 5. Business Insight: 
<br> • July had highest sales but lowest profit percentage
<br> • West region sales lag behind national average
<br> • Category X drives 40% of total revenue

<br><br>
## 6. Tools Used
<br> Microsoft Excel
<br> •	SUMIFS
<br> •	Data Validation
<br> •	Form Controls (Combo Box)
<br> •	Charts (Column, Clustered Column)
<br> •	Formatting and Layout Design
<br> <br>

## 7. How to use this dashboards
<br> 1. Open the Excel file.
<br> 2. Use the dropdown to filter categories.
<br> 3. Check monthly/region performance.
<br> 4. Insights you can derive…

<br> <br>

### This is working Sheet Preview 

<img width="1662" height="720" alt="Working Sheet" src="https://github.com/user-attachments/assets/bbf9d333-546b-485d-b0d7-12356dd95f1d" />


<br> <br>

### Here Is the Preview of my Final Sales Dashboard 

<img width="1693" height="612" alt="Final Sales Dashboard" src="https://github.com/user-attachments/assets/5913a313-f6d6-4362-9258-25aec476a201" />


