# Data Virtualisation  For Business Analysis Denodo-

This project applies data virtualisation techniques using Denodo to address a real-world retail problem: the lack of visibility into whether inventory levels across multiple stores align with actual customer demand.

Using multiple CSV datasets (orders, order items, products, categories, brands, stocks, and stores), I designed a layered virtual data model consisting of base views, integrated views, and an aggregation view. Sales demand, inventory levels, product attributes, brand context, and store information were progressively combined without physically moving data. Feature engineering was applied to derive meaningful business indicators such as stock gap and stock status, translating raw transactional data into actionable insights.

The final report view provides a store-level, near real-time comparison of demand versus stock, allowing identification of overstocked, low-stock, and balanced products across locations. This directly supports better inventory planning, reduces inefficiencies caused by excess stock, and improves product availability where demand exists.

To operationalise the solution, the final view was exposed as a REST API, enabling store-specific queries through simple HTTP requests. This demonstrates how virtualised analytical views can be reused by external systems and dashboards to support faster, data-driven decision-making.

Key tools & concepts: Denodo, data virtualisation, data modelling, feature engineering, REST services, inventory optimisation
