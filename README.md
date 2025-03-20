# Pizza-Sales-Analysis (In Tableau Method)

Data Source:

- **Dataset Used: Pizza Sales data (Date Range: 01-01-2015 to 31-12-2015)**
- **Attributes Included: Order ID, Order Date, Pizza Name, Pizza Category, Pizza Size, Quantity, Price, Total Price, etc.**

Data Modeling:
<br>
Data modeling involves structuring the raw dataset to make it suitable for analysis:

- **Imported the Pizza Sales dataset into Tableau.**
- **Ensured that the data types for fields like:**
   - **Order Date → Date format**
   - **Quantity, Total Price → Integer & Float**
   - **Pizza Category, Pizza Size, Pizza Name → String (Categorical)**
- **Created logical relationships (joins/relationships not shown here) if required, but in this case, a single clean table sufficed.**
- **Used calculated fields such as:**
   - **Avg Order Value = SUM(Total Price) / COUNTD(Order ID)**
   - **Avg Pizzas per Order = SUM(Quantity) / COUNTD(Order ID)**

Data Cleaning:

Cleaning process was performed during data preparation:
- **Handled null values or blanks by:**
   - **Removing empty orders or incomplete rows.**
- **Standardized category names like "Classic", "Supreme", "Veggie", etc.**
- **Removed unnecessary columns which were not useful for visualization.**
- **Ensured consistency in Pizza names (e.g., trimmed extra spaces, corrected naming inconsistencies).**

Data Processing:
<br>
Processing steps included:

- **Aggregated key metrics:**
   - **Total Revenue**
   - **Total Orders**
   - **Total Pizzas Sold**
   - **Average Order Value**
- **Generated Week Number and Hour columns from the Order Date for trend analysis:**
   - **ISO week numbers used for weekly trend chart.**
   - **Extracted hour from Order Date timestamp for hourly analysis.**
- **Created calculated fields for KPI banners (Total Revenue, Orders, Avg Order Value, etc.).**
- **Derived custom fields for Top 5 & Bottom 5 pizzas by Revenue, Quantity, Orders.**

Data Visualization:
<br>
Utilized Tableau’s powerful visualization capabilities to build an interactive dashboard:

Home Dashboard (Image 1):

  - **KPI Metrics:**
  - **Total Revenue: $817.9K**
  - **Avg Order Value: $38.3**
  - **Total Pizzas Sold: 49.6K**
  - **Total Orders: 21.4K**
  - **Avg Pizzas per Order: 2.32**
- **Trend Charts:**
  - **Hourly Trend of Pizzas Sold (Bar Chart) - Identifies peak hours (12 PM - 1 PM & 4 PM - 7 PM).**
  - **Weekly Trend of Total Orders (Line Chart) - Displays order trend across weeks.**
- **Category-wise Sales:**
  - **Pie Chart showing % sales by Pizza Category (Chicken, Veggie, Supreme, Classic).**
  - **Bar Chart showing % sales by Pizza Size (Large, Medium, Small, X-Large).**
- **Order & Pizza Sales by Category - Dual bar chart comparing total pizzas sold vs total orders.**

Analysis and create a dashboard report.

Dashboard Interaction <a href="https://github.com/Moinkhan123456/Pizza-Sales-Analysis/blob/main/Screenshot%20(5).png">View Pizza Sales Report</a>

Dashboard Interaction <a href="https://github.com/Moinkhan123456/Pizza-Sales-Analysis/blob/main/Screenshot%20(6).png">View Best Sale Workers</a>
