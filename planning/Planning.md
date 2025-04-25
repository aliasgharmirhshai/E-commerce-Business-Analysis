
# Plan

Here we discuss data analysis strategy.

# Analytical questions

## Overall Revenue & Volume

### Key Metrics 

- Total Revenue 
- Total Orders 
- Average Order Value (AOV)
- Revenue Over Time (weekly/monthly trend)
- Orders by Payment Type


### Questions

- **Total Revenue Over Time**  
    - What is our total sales value (sum of `payment_value`) by day/week/month?  
    - Tables: `order_payments`, `orders`

- **Total Number of Orders**  
    - How many orders did we receive in each period?  
    - Tables: `orders`

- **Average Order Value (AOV)**  
    - What is the average spend per order? (`sum(payment_value)` ÷ `count(order_id)`)  
    - Tables: `order_payments`, `orders`


## Product & Category Insights

### Metrics

- Top-Selling Products (order_items.price)
- Revenue by Product Category (join products with product_category_name_translation)
- Average Review Score by Product/Category
- Return/Churn Risk by Product
- Product Freight Cost vs. Weight/Size (optimize logistics)

### Questions

- **Top-Selling Product Categories**  
    - Which `product_category_name_english` generate the most revenue?  
    - Tables: `order_items`, `products`, `product_category_name_translation`

- **Best- and Worst-Performing Products**  
    - Which individual products (by `product_id`) have the highest and lowest total sales?  
    - Tables: `order_items`, `products`

- **Price Distribution by Category**  
    - How does item price distribution vary across categories?  
    - Tables: `order_items`, `products`, `product_category_name_translation`

## Geographical Performance

### Key Metrics

- Revenue by State/City
- Customer vs. Seller State Matching (local fulfillment rate)
- Churn Rate by State
- Average Delivery Time by Region
- Freight Cost vs. Distance (join geolocation, use lat/lng to calculate)

### Questions

- **Revenue by State / City**  
    - Which customer states (`customer_state`) drive the most sales?  
    - Tables: `orders`, `order_payments`, `customers`

