# excel-retail-sales-dashboard
Retail sales analysis using Excel pivot tables, VLOOKUP, and dashboard visualization.

## Step 1 – Inspect Dataset
- Opened the dataset and reviewed columns such as Order ID, Product Name, Category, Region, Sales, Quantity, Profit.
- Checked data types for correctness (dates, numbers, text).  

## Step 2 – Data Cleaning
**Remove duplicates:**  
- Used the built-in function Remove Duplicates (often found in Data → Data Tools) to remove repeated rows.
- scs

**Check for missing values:**  
- Filtered each column to find blanks with Data -> Filter (if there are blanks, it is possible to filter columns that contain it)  
- Filled missing numerical values with the arithmetic mean
- Filled missing categorical values with the mode
- -scs

**Add Revenue column:**  
- Formula used: `=Quantity * Sales`  
- Screenshot:  
![Revenue Column](screenshots/revenue_column.png)

## Step 3 – Lookup / Merge Data
- Used VLOOKUP/XLOOKUP to bring Product information (Category, Supplier) into main sales table  
- Screenshot:  
![VLOOKUP Example](screenshots/vlookup_example.png)

## Step 4 – Pivot Tables
**Pivot Table 1:** Revenue by Region  
- Rows: Region  
- Values: Sum of Revenue  
- Screenshot:  
![Pivot Table by Region](screenshots/pivot_table_region.png)

**Pivot Table 2:** Revenue by Category  
- Rows: Category  
- Values: Sum of Revenue  
- Screenshot:  
![Pivot Table by Category](screenshots/pivot_table_category.png)

**Pivot Table 3:** Monthly Sales Trend  
- Rows: Month (from Order Date)  
- Values: Sum of Revenue  
- Screenshot:  
![Pivot Table by Month](screenshots/pivot_table_month.png)

## Step 5 – Dashboard Creation
- Created a new sheet called **Dashboard**  
- Added charts: bar chart for region, column/pie chart for category, line chart for monthly trend  
- Added slicers for Region and Category to make it interactive  
- Screenshot:  
![Dashboard Screenshot](screenshots/dashboard.png)

## Step 6 – Key Insights
- West region generated the highest revenue  
- Electronics category contributed most to sales  
- Sales peak in November–December, suggesting seasonal demand
