# Pizza-Sales-Analysis

Data Source:
<br>
Dataset Used: Pizza Sales data (Date Range: 01-01-2015 to 31-12-2015)
Attributes Included: Order ID, Order Date, Pizza Name, Pizza Category, Pizza Size, Quantity, Price, Total Price, etc.

Data Modeling:
<br> Data modeling involves structuring the raw dataset to make it suitable for analysis:

Imported the Pizza Sales dataset into Tableau.
Ensured that the data types for fields like:
Order Date → Date format
Quantity, Total Price → Integer & Float
Pizza Category, Pizza Size, Pizza Name → String (Categorical)
Created logical relationships (joins/relationships not shown here) if required, but in this case, a single clean table sufficed.
Used calculated fields such as:
Avg Order Value = SUM(Total Price) / COUNTD(Order ID)
Avg Pizzas per Order = SUM(Quantity) / COUNTD(Order ID)

Analysis and create a dashboard report.
