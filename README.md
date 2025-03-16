# Pizza-Sales-Analysis


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pizza Sales Analysis Dashboard</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
            line-height: 1.6;
            margin: 20px;
        }
        h1, h2, h3 {
            color: #d35400;
        }
        h1 {
            text-align: center;
        }
        ul, ol {
            margin-left: 20px;
        }
        code {
            background-color: #f4f4f4;
            padding: 2px 4px;
            border-radius: 4px;
        }
        .section {
            background-color: #fff;
            padding: 15px;
            margin-bottom: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .folder-structure {
            background-color: #f0f0f0;
            padding: 10px;
            border-radius: 6px;
            font-family: monospace;
        }
    </style>
</head>
<body>

    <h1>🍕 Pizza Sales Analysis Dashboard</h1>
    <h3>End-to-End Data Analytics Project (Tableau)</h3>

    <div class="section">
        <h2>📂 Data Source:</h2>
        <ul>
            <li><strong>Dataset Used:</strong> Pizza Sales data (Date Range: 01-01-2015 to 31-12-2015)</li>
            <li><strong>Attributes Included:</strong> Order ID, Order Date, Pizza Name, Pizza Category, Pizza Size, Quantity, Price, Total Price, etc.</li>
        </ul>
    </div>

    <div class="section">
        <h2>🏗️ 1. Data Modeling:</h2>
        <ul>
            <li>Imported the Pizza Sales dataset into Tableau.</li>
            <li>Ensured correct data types:
                <ul>
                    <li><code>Order Date</code> → Date format</li>
                    <li><code>Quantity</code>, <code>Total Price</code> → Integer & Float</li>
                    <li><code>Pizza Category</code>, <code>Pizza Size</code>, <code>Pizza Name</code> → String</li>
                </ul>
            </li>
            <li>Created calculated fields such as:
                <ul>
                    <li><strong>Avg Order Value =</strong> SUM(Total Price) / COUNTD(Order ID)</li>
                    <li><strong>Avg Pizzas per Order =</strong> SUM(Quantity) / COUNTD(Order ID)</li>
                </ul>
            </li>
        </ul>
    </div>

    <div class="section">
        <h2>🧹 2. Data Cleaning:</h2>
        <ul>
            <li>Removed null values or blanks from dataset.</li>
            <li>Standardized pizza category names (Chicken, Classic, Veggie, Supreme).</li>
            <li>Removed unnecessary columns.</li>
            <li>Cleaned Pizza names for consistency (trimmed spaces, corrected spellings).</li>
        </ul>
    </div>

    <div class="section">
        <h2>⚙️ 3. Data Processing:</h2>
        <ul>
            <li>Aggregated key metrics:
                <ul>
                    <li>Total Revenue</li>
                    <li>Total Orders</li>
                    <li>Total Pizzas Sold</li>
                    <li>Average Order Value</li>
                </ul>
            </li>
            <li>Extracted Week Number and Hour from Order Date for trend analysis.</li>
            <li>Derived custom fields for:
                <ul>
                    <li>Top 5 & Bottom 5 Pizzas by Revenue</li>
                    <li>Top 5 & Bottom 5 Pizzas by Quantity</li>
                    <li>Top 5 & Bottom 5 Pizzas by Total Orders</li>
                </ul>
            </li>
        </ul>
    </div>

    <div class="section">
        <h2>📊 4. Data Visualization:</h2>
        <p>Utilized Tableau to build an interactive dashboard:</p>
        <h3>Home Dashboard:</h3>
        <ul>
            <li><strong>KPI Metrics:</strong> Total Revenue, Avg Order Value, Total Pizzas Sold, Total Orders, Avg Pizzas per Order.</li>
            <li><strong>Hourly Trend of Pizzas Sold:</strong> Bar Chart showing peak order hours.</li>
            <li><strong>Weekly Trend of Total Orders:</strong> Line Chart showing order flow.</li>
            <li><strong>Category-wise Sales:</strong>
                <ul>
                    <li>Pie Chart for Pizza Category % Sales.</li>
                    <li>Bar Chart for Pizza Size % Sales.</li>
                </ul>
            </li>
            <li>Dual Bar Chart comparing Total Pizzas Sold vs Total Orders by Category.</li>
        </ul>

        <h3>Best/Worst Sellers Dashboard:</h3>
        <ul>
            <li>Top 5 Pizzas by Revenue, Quantity, and Total Orders.</li>
            <li>Bottom 5 Pizzas by Revenue, Quantity, and Total Orders.</li>
            <li>Text Annotations explaining key insights.</li>
        </ul>

        <h3>Tableau Features Used:</h3>
        <ul>
            <li>KPI Banners (Pulse Metrics)</li>
            <li>Bar, Line, Pie Charts</li>
            <li>Dual-axis Charts</li>
            <li>Calculated Fields</li>
            <li>Filters (Pizza Category, Date Range)</li>
            <li>Dashboard Interactions & Actions</li>
        </ul>
    </div>

    <div class="section">
        <h2>🚀 Deployment Steps:</h2>
        <ol>
            <li>Prepared dataset in Excel/CSV.</li>
            <li>Imported dataset into Tableau Public.</li>
            <li>Performed data cleaning, calculated fields, and data modeling.</li>
            <li>Created visualizations & KPI dashboards.</li>
            <li>Published dashboard to Tableau Public / Exported as .twbx file.</li>
            <li>Documented process and added screenshots + dataset to GitHub.</li>
        </ol>
    </div>

</body>
</html>


Analysis and create a dashboard report.

Dashboard Interaction <a href="https://github.com/Moinkhan123456/Pizza-Sales-Analysis/blob/main/Screenshot%20(5).png">View Pizza Sales Report</a>

Dashboard Interaction <a href="https://github.com/Moinkhan123456/Pizza-Sales-Analysis/blob/main/Screenshot%20(6).png">View Best Sale Workers</a>
