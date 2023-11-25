# project-playground

## Requirements:
- User Authentication and Authorization:
- Requirement: Secure login for inventory managers with role-based access.
Database Source: User management table in the authentication database.

- Real-Time Inventory Overview:
Requirement: Immediate visibility into the current stock levels for all products.
Database Source: Transactional database containing real-time stock data.

- Product Details and Attributes:
Requirement: Access to detailed information about each product, including descriptions and specifications.
Database Source: Product information table in the inventory database.

- Sales and Purchase History:
Requirement: Historical data on sales and purchases to analyze trends and patterns.
Database Source: Sales transactions and purchase orders tables in the transactional database.

- Stock-Out Alerts:
Requirement: Notifications or alerts for stock-out situations.
Database Source: Inventory management system logging stock-out events.

- Supplier Information:
Requirement: Details on suppliers, delivery schedules, and contact information.
Database Source: Supplier information table in the inventory database.

- Order Processing Status:
Requirement: Tracking the status of open orders and shipments.
Database Source: Order status table in the order processing database.

- Financial Metrics:
Requirement: Monitor the cost of goods sold (COGS), profit margins, and overall financial performance.
Database Source: Sales transactions, purchase orders, and financial data tables.

## KPIs and Metrics:
Inventory Turnover Rate:
KPI: How quickly products are sold and restocked.
Metric: Inventory turnover ratio.
Source Tables: Sales transactions, product information, and inventory data.

Stock-Out Rate:
KPI: Frequency of stock-outs.
Metric: Stock-out rate percentage.
Source Tables: Sales transactions, inventory data, and stock-out logs.

Order Fulfillment Time:
KPI: Efficiency in processing and fulfilling orders.
Metric: Average time from order placement to shipment.
Source Tables: Order processing status and timestamps.

Product Profitability:
KPI: Identify the most and least profitable products.
Metric: Gross profit margin per product.
Source Tables: Sales transactions and cost data.

Supplier Performance:
KPI: Evaluate supplier reliability and efficiency.
Metric: On-time delivery rate.
Source Tables: Supplier information, purchase orders, and delivery data.
