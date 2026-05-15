📌 Project Overview
This project presents an end-to-end interactive sales dashboard built in Microsoft Power BI, analyzing mobile phone sales data sourced from Kaggle. The dashboard enables business stakeholders to monitor sales performance across cities, brands, models, and payment methods — and make data-driven decisions around inventory, pricing, and regional strategy.
Dataset: 10,000+ rows of mobile sales transaction data
Source: Kaggle
Tools: Power BI, DAX, Data Modeling (Star Schema)

🎯 Business Problem
Retail and e-commerce businesses selling mobile phones often struggle to answer:

Which cities and brands are driving the most revenue?
When do sales peak — and why?
Which payment methods do customers prefer?
Which models are underperforming and need attention?

This dashboard answers all of these questions in one place.

📊 Dashboard Features
The dashboard contains 6–8 interactive visuals including:
VisualPurposeTotal Sales KPI CardOverall revenue at a glanceUnits Sold KPI CardVolume of transactionsCity-wise Sales Map / Bar ChartRegional performance comparisonBrand & Model Performance ChartTop and bottom performing modelsMonthly Sales Trend Line ChartSeasonality and peak period analysisPayment Method Breakdown (Donut)Customer payment preference analysisDynamic SlicersFilter by city, brand, model, month

🔍 Key Findings & Business Insights

These insights were derived directly from the data — not assumptions.


📍 Delhi recorded the highest mobile sales among all cities, making it the most critical market for inventory prioritization and targeted marketing campaigns.
📱 iPhone was the top-selling brand, consistently outperforming Android competitors across multiple cities — indicating strong brand loyalty and premium segment demand.
💳 UPI was the most preferred payment method, accounting for the majority of transactions — suggesting the customer base is digitally active and businesses should ensure seamless UPI checkout experiences.
📈 Sales peaked in March, likely driven by end-of-financial-year purchases, salary cycles, and seasonal promotions — recommending businesses stock up inventory ahead of Q1 end.
🏙️ City-wise analysis revealed significant variation in brand preference by region, enabling location-specific marketing and stocking decisions.


🛠️ Technical Implementation
Data Modeling

Designed a star schema with fact and dimension tables for clean, optimized reporting
Established relationships between sales, product, city, and date tables

DAX Measures Used
Total Revenue = SUM(Sales[Revenue])
Total Units Sold = COUNT(Sales[TransactionID])
Average Selling Price = DIVIDE([Total Revenue], [Total Units Sold])
MoM Growth % = DIVIDE([Current Month Sales] - [Last Month Sales], [Last Month Sales]) * 100
Top City = CALCULATE([Total Revenue], TOPN(1, Cities, [Total Revenue]))
Data Cleaning Steps

Removed null and duplicate transaction records
Standardized city names and brand names for consistent grouping
Converted date columns to proper date format for time intelligence functions
Validated revenue figures against units sold × price


📸 Dashboard Screenshots

(Add screenshots of your Power BI dashboard here)
Tip: Export from Power BI → File → Export → PNG, then drag into this README on GitHub


🚀 How to Use This Project

Clone or download this repository
Open MS_Dashboard-.pbix in Microsoft Power BI Desktop (free download)
Explore the dashboard using slicers to filter by city, brand, model, or month
Review DAX measures in the Model View for formula logic


📁 Project Structure
mobile-sales-dashboard/
│
├── MS_Dashboard-.pbix        # Power BI Dashboard file
├── README.md                 # Project documentation
└── Screenshots/              # Dashboard preview images

💡 Skills Demonstrated

✅ Data Cleaning & Transformation
✅ Star Schema Data Modeling
✅ DAX Measures & Calculated Columns
✅ KPI Dashboard Design
✅ Business Insight Extraction
✅ Interactive Filters & Drill-Through


👤 Author
Kamlesh Mhaske
Aspiring Data Analyst | SQL · Python · Power BI · Excel
📧 kamleshmhaske16@gmail.com
🔗 LinkedIn | GitHub
