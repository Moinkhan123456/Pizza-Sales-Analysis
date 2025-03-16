# Pizza-Sales-Analysis

1.Data Source:
<br>
Dataset Used: Pizza Sales data (Date Range: 01-01-2015 to 31-12-2015)
<br>
Attributes Included: Order ID, Order Date, Pizza Name, Pizza Category, Pizza Size, Quantity, Price, Total Price, etc.

2.Data Modeling:
<br>
Data modeling involves structuring the raw dataset to make it suitable for analysis:
<br>
Imported the Pizza Sales dataset into Tableau.
<br>
Ensured that the data types for fields like:
<br>
Order Date → Date format
<br>
Quantity, Total Price → Integer & Float
<br>
Pizza Category, Pizza Size, Pizza Name → String (Categorical)
<br>
Created logical relationships (joins/relationships not shown here) if required, but in this case, a single clean table sufficed.
<br>
Used calculated fields such as:
<br>
Avg Order Value = SUM(Total Price) / COUNTD(Order ID)
<br>
Avg Pizzas per Order = SUM(Quantity) / COUNTD(Order ID)

3.Data Cleaning:
<br>
Cleaning process was performed during data preparation:
<br>
Handled null values or blanks by:
<br>
Removing empty orders or incomplete rows.
<br>
Standardized category names like "Classic", "Supreme", "Veggie", etc.
<br>
Removed unnecessary columns which were not useful for visualization.
<br>
Ensured consistency in Pizza names (e.g., trimmed extra spaces, corrected naming inconsistencies).


Analysis and create a dashboard report.

Dashboard Interaction <a href="https://github.com/Moinkhan123456/Pizza-Sales-Analysis/blob/main/Screenshot%20(5).png">View Pizza Sales Report</a>

Dashboard Interaction <a href="https://github.com/Moinkhan123456/Pizza-Sales-Analysis/blob/main/Screenshot%20(6).png">View Best Sale Workers</a>
