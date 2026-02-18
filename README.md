# Instacart Grocery Orders — PostgreSQL Data Analysis
Project Overview

In this project, I analyzed customer purchasing behavior using the Instacart online grocery dataset in PostgreSQL. My objective was to uncover patterns in reordering behavior, department performance, shopping frequency, and product affinity to generate insights that could support customer retention, staffing optimization, and personalized marketing strategies.

Through structured SQL analysis across millions of transactional records, I evaluated how customers behave across first-time and repeat purchases, which products drive loyalty, and how timing influences demand patterns.

---

## Project Objectives
In this analysis, I aimed to answer the following business questions:
1. Which products are most frequently reordered, and what does this indicate about customer loyalty?
2. How do the top 10 most purchased products during first orders differ from subsequent orders?
3. Which department contributes the most to product sales, and is this consistent across weekdays?
4. What are the busiest days and hours for orders, and how can this influence staffing or marketing?
5. How frequently do customers place repeat orders, and how does this vary among top shoppers?
6. What product pairs are frequently reordered together, and how can this support bundling strategies?
7. Which department has the highest and lowest reorder ratios, and what might this reveal?
8. Are customers more likely to reorder at certain times or days?
9. Who are the most active customers, and what can their behavior tell us about high-value segments?

---

## Tools & Technical Approach
In this project, I used:
- PostgreSQL
- Common Table Expressions (CTEs) to break down multi-step behavioral analysis
- Aggregate functions (COUNT, SUM, AVG) to measure reorder frequency and department contribution
- CASE statements to segment first-time vs repeat orders
- JOINs across orders, products, aisles, and departments tables
- FILTER clauses for conditional aggregations
- Window functions (ROW_NUMBER, ranking logic) to identify top customers and products
- Time-based analysis using hour-of-day and day-of-week grouping

Because the dataset included millions of rows, I carefully structured queries to avoid unnecessary subqueries and ensure performance efficiency.

---

## Key Insights / Results
Through this analysis, I identified:
- Bananas, organic strawberries, and baby spinach are among the most reordered products, reflecting strong repeat demand and habitual purchasing behavior.
- First-time customers tend to focus on essentials, while repeat orders include more diverse and specialty items.
- The produce department contributes the largest share of total sales, particularly on weekends.
- Order volume peaks between 10 AM and 4 PM, with highest activity on Sunday and Monday.
- The top 10% of customers order significantly more frequently and exhibit stronger reorder patterns, representing high-value loyalty segments.
- Certain product combinations (e.g., chips & salsa, yogurt & granola) show strong co-reorder behavior, suggesting bundling or recommendation opportunities.
- Some departments (e.g., dairy) show reorder ratios exceeding 70%, while others (e.g., baby or personal care) have lower repeat behavior, indicating potential promotional opportunities.

This analysis demonstrates how transactional grocery data can be leveraged to improve customer retention strategies, optimize staffing schedules, enhance cross-selling recommendations, and prioritize high-loyalty product categories.

---

## What I Learned
Through this project, I strengthened my ability to:
- Analyze large-scale transactional datasets in PostgreSQL
- Measure and interpret customer loyalty using reorder ratios
- Perform behavioral segmentation between first-time and repeat customers
- Identify product affinity patterns for bundling strategies
- Translate time-based ordering behavior into operational recommendations

I also gained deeper insight into how e-commerce grocery platforms use behavioral data to drive growth and retention.This dataset includes over 3 million grocery orders from more than 200,000 users, covering:

---

## Challenges I Encountered
One challenge I faced was efficiently analyzing reorder ratios across millions of records. I addressed this by using CTEs and conditional aggregations rather than nested subqueries.

Another challenge involved identifying meaningful product pair combinations without inflating co-occurrence counts. I carefully structured self-joins and grouping logic to avoid duplication.

Additionally, interpreting reorder patterns required thoughtful segmentation between habitual purchases and occasional items to avoid misleading conclusions.

---

## Dataset Overview
This dataset contains over 3 million grocery orders from more than 200,000 users, including:

- Products
- Aisles and Departments
- Orders (train and prior)
- Order timing (day of week, hour of day)
- Reorder indicators

