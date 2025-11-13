# BWM-SALES-DASHBOARD
🚗 BMW Sales Power BI Dashboard 📊 Project Overview  This project presents an interactive Power BI dashboard that visualizes and analyzes BMW car sales performance across various regions, models, and sales channels. It helps business users understand sales trends, top-performing models, and market insights to support data-driven decision
🧩 Dataset Details

The dataset contains key information related to BMW sales:

Column Name	Description
Date	Transaction date of sale
Year	Year of the sale
Model	BMW car model name
Revenue	Total revenue generated from the sale
Quantity Sold	Number of cars sold
Region	Geographic region (e.g., Europe, Asia, America)
Country	Country of sale
Channel	Sales channel (e.g., Dealer, Online)
📈 Key Measures (DAX)

The following DAX measures were created for insightful analysis:
Total Sales = SUM(Revenue)
Total Quantity Sold = SUM(Quantity Sold)
Average Selling Price = DIVIDE([Total Sales], [Total Quantity Sold])
Max Priced Model = MAXX(TOPN(1, BMW_Sales_Data, BMW_Sales_Data[Revenue], DESC), BMW_Sales_Data[Model])
Highest Selling Model = MAXX(TOPN(1, BMW_Sales_Data, BMW_Sales_Data[Quantity Sold], DESC), BMW_Sales_Data[Model])
Sales Growth % (YoY) = Compare current year sales with previous year

Sales by Channel / Region / Model
🖥️ Dashboard Features
Interactive filters by Year, Country, Model, and Channel
KPIs showing Total Sales, Quantity Sold, Avg Price, Growth %
Map visualization for regional sales
Bar charts for sales by model and channel
Dynamic cards showing Top-selling and Max-priced models

🧠 Insights
Identifies the best-performing BMW model and top revenue regions.
Tracks sales growth trends over time.
Highlights which sales channels contribute most to total revenue.

⚙️ Tools Used
Power BI Desktop
Microsoft Excel / CSV (for dataset)
DAX (Data Analysis Expressions)
GitHub (for version control and sharing)

📚 How to Use

Download the .pbix file or clone this repository.
Open in Power BI Desktop.
Load the dataset and refresh the visuals.
Explore the dashboard interactively.

🏁 Conclusion
The BMW Sales Dashboard provides a complete view of the company’s sales performance across different dimensions. It can assist business teams, dealers, and management in making informed decisions about production, marketing, and regional strategies.
