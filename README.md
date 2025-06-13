# Inventory_Analysis
![image](https://github.com/user-attachments/assets/79b2a910-7f9a-4389-89e2-71d0f1a6a01e)


 **Project Overview**

Urban Retail Co. is a growing mid-sized retail chain operating across various regions, offering a diverse range of products. Despite access to a robust data infrastructure, the company was facing persistent inventory inefficiencies: certain products were chronically overstocked, some critical items were frequently understocked, and warehouse-level imbalances were leading to customer dissatisfaction and lost revenue opportunities.
In this project, I took on the role of a data analyst tasked with diagnosing and addressing these inefficiencies. The solution involved building a comprehensive SQL-based data pipeline to calculate essential KPIs, followed by designing dynamic Power BI dashboards that would help business stakeholders make data-informed decisions. The ultimate goal was to shift Urban Retail Co. from a reactive inventory model to a proactive, analytics-driven strategy.

 **Business Objective**
 
The main objective was to improve inventory visibility, optimize product movement, and enhance stock allocation across stores and regions. This was achieved by analyzing fast-moving vs. slow-moving products, identifying understocked and overstocked regions, calculating turnover rates, and evaluating the accuracy of the company’s demand forecasting system.
By transforming raw sales, inventory, and product movement data into actionable insights, this project aimed to help the company reduce working capital tied up in excess stock, avoid lost sales due to stockouts, and ensure that the right products were always in the right place at the right time.

 **Tools & Technologies**
 
To execute the project effectively, I used SQL (MySQL) for all back-end data processing. This included cleaning and merging multiple datasets, computing custom KPIs like inventory turnover and forecast accuracy, and segmenting products based on performance. The processed data was then visualized using Power BI, which allowed the creation of highly interactive dashboards capable of filtering data by category, region, and time period.
Python and Excel were also used for preliminary tagging and validating movement classifications. These tools were particularly helpful for determining fast vs. slow-moving products based on turnover benchmarks and average revenue values.

 **Dataset Overview**

The analysis was built upon four key datasets:
stocklevel regions.csv: Provides product-level inventory figures across different regions.


stocklevel stores.csv: Captures inventory data at the individual store level.


Fast moving.csv: Contains detailed metrics including revenue, units sold, average inventory value, and inventory turnover ratio. It also includes a movement category column, tagging products as fast- or slow-moving.


low inventory regions.csv: Flags historical incidents of stockouts by region, date, and product.


These datasets were merged and processed to create a comprehensive view of inventory health across the organization.

 **Key Metrics and Findings**
 
One of the central metrics used in this analysis was the Inventory Turnover Ratio, which represents how efficiently a product is being sold and replenished over a period. The average turnover across all products was approximately 1210.02, with fast-moving items like P0046, P0133, and P0057 performing significantly above this benchmark. These products also contributed the highest revenues, each averaging over ₹10 million.
In contrast, slow-moving products such as P0070 and P0068 had lower turnover ratios (below 1160) despite having moderately high revenue. This indicated that while they were valuable items, their storage and holding costs were disproportionately high due to slower inventory movement.
Another key discovery was the high number of stockouts in stores like S002, S001, and S004. These stores frequently appeared in the low-inventory alerts and required immediate attention to avoid revenue loss due to unfulfilled demand.
Forecast accuracy was another crucial dimension of the project. The organization’s existing demand forecasts were shown to be accurate on average (~88%), but the analysis revealed that this accuracy dropped in specific product categories and store combinations — highlighting the need for more granular forecasting at the store level.

 **Dashboard & Visual Insights**

To support decision-making, I designed a series of Power BI dashboards that transformed SQL metrics into business-friendly visuals:
Units Sold by Quarter and Category: Tracked seasonal trends, showing consistent high sales in Clothing and Groceries.

Inventory Levels by Category: Identified overstocking in Furniture and Electronics and lean inventory in Toys.

Forecast Accuracy Comparison: Validated prediction models across categories, uncovering gaps at a micro level.

Inventory Turnover by Category: Showed which categories were driving revenue vs. those holding back capital.

Fast vs. Slow-Moving Products: A segmentation dashboard to drive marketing and stocking decisions.

Regional Stock Heatmaps: Provided a clear view of overstock and understock across North, South, East, and West regions.

These visuals were designed to be interactive, enabling users to slice and drill down by region, product ID, and time period.

 **Business Insights**

This analysis led to several key insights:
Overstocking in High-Cost Categories: Electronics and Furniture had substantial excess stock in the North and South regions, suggesting a need for better demand planning or inventory redistribution.


Frequent Stockouts in High-Demand Categories: Toys and Electronics consistently showed low inventory in the West region, pointing to poor supply chain alignment with actual regional demand.


High Turnover Categories: Clothing and Groceries emerged as the fastest-moving product lines and should be prioritized in stocking and replenishment decisions.


Slow Movers with High Value: Despite their revenue potential, items like P0070 had poor turnover and should be considered for promotional campaigns or bundling offers.


Forecasting Blind Spots: While category-level forecasts appeared accurate, discrepancies at the store level suggested the need for more granular modeling.



**Strategic Recommendations**

Based on the above insights, I proposed the following actions for Urban Retail Co.:
Reorganize Inventory Distribution: Shift excess stock from overstocked regions (North, South) to regions with consistent stockouts (West), especially for high-margin products like Electronics.

Revise Reorder Policies: Automate restocking decisions using turnover-based thresholds rather than static rules, allowing the system to adapt to dynamic sales trends.

Run Targeted Promotions for Slow Movers: Launch offers or bundles for low-turnover but high-value products to reduce holding costs and free up storage space.

Enhance Forecasting Models: Develop store-level forecasting systems to account for regional variation in demand patterns, ensuring greater accuracy and reduced mismatch.

Implement Weekly Monitoring Dashboards: Use Power BI to monitor KPIs like turnover, inventory levels, and stockouts on a weekly basis to stay ahead of potential issues.
