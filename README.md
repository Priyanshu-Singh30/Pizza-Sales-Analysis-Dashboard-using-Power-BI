# Pizza-Sales-Analysis-Dashboard-using-Power-BI
## Project Objective
The objective of the Pizza Sales Dashboard project is to analyze and visualize sales performance of a pizza store using transactional data. This includes identifying key trends such as total revenue, total revenue by category, pizza orders by month, pizza size etc. The insights are presented using interactive visuals in Power BI to help management make data-driven decisions for inventory planning, marketing, and sales optimization.
## Dataset Used
- Dataset <a href="https://github.com/Priyanshu-Singh30/Pizza-Sales-Analysis-Dashboard-using-Power-BI/blob/main/pizza_sales%20(1)%20(1).zip">Dataset view</a>
- Dashboard Interaction <a href="https://github.com/Priyanshu-Singh30/Pizza-Sales-Analysis-Dashboard-using-Power-BI/blob/main/Pizza_Sales01.pbix">Dashboard view</a>
## Process
1. Import Data
   - Load 4 CSV files: orders, order_details, pizzas, pizza_types
2. Clean Data (Power Query)
   - Remove nulls, rename columns, set data types
   - Extract Month and Hour from Date and Time
3. Create Relationships
   - Link order_id, pizza_id, and pizza_type_id across tables
4. Create DAX Measures
   - Example:
     - Total Revenue = SUMX(order_details, quantity * RELATED(price))
     - Total Orders = DISTINCTCOUNT(order_id)
5. Build Visuals
   - Card: Total Revenue, Total Orders
   - Bar/Column: Most Ordered Pizzas
   - Donut: Revenue by Category
   - Line: Orders over Time
   - Slicer: Size
## Dashboard
<img width="1304" height="739" alt="Screenshot 2025-08-05 112947" src="https://github.com/user-attachments/assets/0240c36b-c0e3-4dfc-8076-7dd1913d382c" />
