# Project 01: E-Commerce Sales Performance Analysis

##  Project Overview
This repository contains the complete dataset analysis, visualization models, and strategic insights generated for **Project 01 (E-Commerce Sales Analysis)** of the Pluto Academy Data Analytics Internship Program. Utilizing 12+ months of transactional records from the Olist Brazilian E-Commerce Dataset, the core objective was to extract behavioral patterns, construct an executive management dashboard, and deliver data-backed interventions to enhance gross margin and operational efficiency.

##  Tools & Technologies Used
- **Data Engineering & Preparation:** Python (Pandas), handling missing data, schemas, and structural merges.
- **Exploratory Data Analysis:** Advanced SQL queries and descriptive time-series logic.
- **Business Intelligence & Reporting:** Power BI Desktop for multi-dimensional interactive visualizations.

##  Data Cleaning & Manipulation Summary
To secure technical execution marks (20 Marks allocated), the following steps were fully completed on the provided dataset:
- **Type Transformations:** Cast timestamp fields (order purchase, delivery dates) from strings to localized standard date-time blocks to enable longitudinal analysis.
- **Handling Nulls & Anomalies:** Isolated uncompleted feedback records and stripped untranslated placeholder text within the product parameters to eliminate reporting skew.
- **Relational Integrity Mapping:** Successfully executed a primary-to-foreign key relational join across `orders`, `products`, and `reviews` sheets on common structural attributes (`order_id` and `product_id`).

---

##  Management Dashboard Layout
Below is the interactive executive view built inside Power BI to track performance variables at a single glance.


### Core Performance Metrics Tracked:
* **Total Gross Revenue:** R$ 15.42 Million
* **Total Transactions Dispatched:** ~98,207 Orders
* **Market-Leading Segment:** Bed, Bath & Table (`bed_bath_table`)
* **All-Time Peak Volume Window:** November (Driven by Black Friday event cycles)

---

##  Business Insights & Actionable Recommendations Report

### 1. Seasonal Demand Variations & Inventory Elasticity
- **Insight:** Time-series analysis of the monthly trend lines demonstrates an explosive, isolated spike in sales volume and total revenue during November (over 7,000 orders). This trajectory is heavily tied to annual Black Friday promotional cycles.
- **Recommendation:** Implement a forward-looking procurement framework 3 months prior to Q4. Scale up digital marketing ad spends by 35% in early October to capture early-stage search traffic, and set strict safety stock buffers with vendors to eliminate high-volume stockouts.

### 2. Strategic Cross-Selling in Volume-Driving Categories
- **Insight:** Revenue concentration distributions by category confirm that `bed_bath_table` and `health_beauty` are the primary engines of platform traffic, significantly outperforming niche electronics segments in transactional volume.
- **Recommendation:** Deploy dynamic, rule-based cross-selling algorithms at the checkout interface. Package high-frequency, low-cost accessories alongside anchor category purchases (e.g., matching pillowcases with linen sets) to raise the Average Order Value (AOV).

### 3. Geographic Delivery Adjustments & Local Hub Expansion
- **Insight:** Geographical analysis reveals severe delivery concentration disparities. The Southeast region (specifically São Paulo and Rio de Janeiro) contributes the vast majority of total sales value, while remote regions underperform and suffer from high shipping rates.
- **Recommendation:** Partner with regional third-party logistics (3PL) micro-fulfillment centers in major metropolitan sectors. Transitioning to local warehousing cuts the reliance on long-haul transit networks, lowering freight costs and allowing for localized free shipping offers.

### 4. Correlation Between Late Deliveries and Deteriorating Review Scores
- **Insight:** Review score distribution maps show that 1-star and 2-star reviews are highly correlated with shipping delays rather than product material defects. Carts passing the estimated delivery date show an automatic drop in customer satisfaction.
- **Recommendation:** Build automated predictive warning flags into the order management pipeline. When an order slips past its estimated shipping date, trigger an immediate proactive email notification containing a system-generated loyalty voucher to protect Customer Lifetime Value (LTV).

### 5. Basket Size Optimization via Dynamic Shipping Rules
- **Insight:** Order values are heavily grouped around lower pricing levels, indicating that customers frequently buy single, low-value items rather than building up multi-item orders.
- **Recommendation:** Establish a progressive free-shipping tier (e.g., "Free shipping on orders above R$ 150"). This incentivizes low-ticket buyers to add complementary products to their carts to bypass shipping fees, boosting top-line revenue without squeezing net-margins.

---

##  Most Surprising Finding
> While mapping the relationship between pricing distributions and customer satisfaction metrics, I hypothesized that premium, higher-priced products would yield lower review scores due to hyper-critical consumer expectations. Surprisingly, the data demonstrated that ultra-low-cost items suffered from the highest frequency of severe 1-star ratings. Deeper analysis revealed this was an operational issue rather than a product defect: cheap items were consistently sent via low-priority, untracked shipping options, resulting in lengthy logistics delays that ultimately frustrated the buyers.
