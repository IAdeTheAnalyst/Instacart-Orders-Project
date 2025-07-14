🛒 Instacart Grocery Orders — PostgreSQL Data Analysis
This project explores customer purchasing behaviors using Instacart’s online grocery dataset. By analyzing patterns in reordering, department performance, and user behavior across time, this project provides actionable insights into customer loyalty, optimal staffing times, and product bundling.

🧠 Key Business Questions
Which products are most frequently reordered, and what does this indicate about customer loyalty?

How do the top 10 most purchased products during first orders differ from subsequent orders?

Which department contributes the most to product sales, and is this consistent across weekdays?

What are the busiest days and hours for orders, and how can this influence staffing or marketing?

How frequently do customers place repeat orders, and how does this vary among top shoppers?

What product pairs are frequently reordered together, and how can this support bundling strategies?

Which department has the highest and lowest reorder ratios, and what might this reveal?

Are customers more likely to reorder at certain times or days?

Who are the most active customers, and what can their behavior tell us about high-value segments?

📊 Tools Used
SQL (PostgreSQL)

Common Table Expressions (CTEs)

Aggregate Functions

CASE Statements

JOINs & Subqueries

FILTER Clause

Window Functions (e.g., ROW_NUMBER)

📌 Key Insights
Product Loyalty: Bananas, organic strawberries, and baby spinach top the list of most reordered products, suggesting strong brand or item loyalty.

Behavior Shift: First-time buyers focus on essentials like water and produce, but shift toward diverse items in later orders.

Peak Departments: The produce department leads in total sales, especially on weekends, indicating when stock and staff should be reinforced.

Customer Timing: Most orders are placed between 10 AM and 4 PM, with peak days on Sunday and Monday.

Top Shoppers: The most active 10% of users order more frequently and show stronger reorder habits, providing a focus group for loyalty campaigns.

Bundling Opportunities: Items like chips and salsa or yogurt and granola are frequently bought together, supporting personalized recommendations.

Retention Metrics: Some departments have over 70% reorder ratios (e.g., dairy), while others like baby or personal care are much lower—revealing where to improve customer experience or promotions.

📂 Dataset Overview
This dataset includes over 3 million grocery orders from more than 200,000 users, covering:

Products

Aisles & Departments

Orders (train/prior)

Reordering behavior

Day/hour of order

Source: Instacart Market Basket Analysis | Kaggle

