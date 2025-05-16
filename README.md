# supersales_16.05.2025
# 🎯 Top Seller Analysis per Category (SQL)

This SQL project identifies the most popular product in each category based on the total quantity sold.

## 📂 Tables used:
- `products` – contains `product_id`, `product_price`, and `group_id`
- `product_groups` – maps `group_id` to `category`
- `order_positions` – stores `product_id` and `item_quantity` (units sold)

## 🧠 Objective:
For each category:
- Calculate the total number of units sold per product
- Determine the product with the highest sales volume
- Label it as `"Top Seller"` and others as `"Other"`

## 🧩 SQL Logic:
1. Join product data with category info and sales
2. Aggregate item_quantity per product and category
3. Use `ROW_NUMBER()` to rank products within categories
4. Assign label based on ranking
