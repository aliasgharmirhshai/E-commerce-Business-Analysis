# Customer Behavior Analysis

## 1. Product Category & Seller Information
**Tables:** `product_category_name_translation` and `sellers`  
**Key Columns:** `product_category_name`, `product_category_name_english`, `seller_id`, `seller_city`, `seller_state`

### Insights:
- **Category Popularity:** Analyze which product categories customers purchase most often to understand popular product types.
- **Seller Performance:** Identify top-performing sellers based on the number of orders and customer reviews.
- **Geographic Distribution:** Compare seller locations with customer locations to analyze shipping behavior and delivery performance.

---

## 2. Customer Information & Geolocation
**Tables:** `customers` and `geolocation`  
**Key Columns:** `customer_id`, `customer_city`, `customer_state`, `geolocation_lat`, `geolocation_lng`, `geolocation_city`, `geolocation_state`

### Insights:
- **Customer Segmentation:** Use geolocation data to identify trends in customer behavior based on location (e.g., urban vs. rural areas).
- **Shipping & Delivery Insights:** Analyze customer locations against seller zip codes to gauge shipping distance and time, improving regional delivery performance.

---

## 3. Order & Transaction Details
**Tables:** `order_items`, `order_payments`, `orders`  
**Key Columns:** `order_id`, `order_item_id`, `product_id`, `price`, `freight_value`, `payment_type`, `payment_value`, `order_purchase_timestamp`, `order_status`, `order_delivered_customer_date`

### Insights:
- **Product Performance:** Identify frequently purchased product combinations and high-revenue items.
- **Order Conversion Rate:** Track completed versus abandoned orders by analyzing `order_status`.
- **Payment Trends:** Understand payment methods and installment usage to tailor marketing strategies.
- **Customer Purchase Timing:** Analyze timestamps to identify peak purchase times (e.g., specific days or times).

---

## 4. Customer Reviews
**Table:** `order_reviews`  
**Key Columns:** `review_score`, `review_comment_title`, `review_comment_message`

### Insights:
- **Customer Satisfaction:** Use review scores and comments to analyze customer sentiment towards products, sellers, and the overall shopping experience.
- **Common Pain Points:** Identify recurring issues from negative reviews to improve products or customer service.

---

## 5. Lead Data (for B2B or CRM Analysis)
**Tables:** `leads_qualified` and `leads_closed`  
**Key Columns:** `mql_id`, `first_contact_date`, `origin`, `won_date`, `business_segment`, `lead_type`, `lead_behaviour_profile`

### Insights:
- **Lead Conversion:** Track lead conversion speed and identify segments or profiles with higher conversion rates.
- **Lead Source:** Determine which lead sources generate high-value customers.
- **Business Segmentation:** Analyze whether specific business types (e.g., small vs. large enterprises) are more likely to convert.

---

## 6. Product and Shipping Characteristics
**Table:** `products`  
**Key Columns:** `product_name_lenght`, `product_description_lenght`, `product_photos_qty`, `product_weight_g`, `product_length_cm`, `product_height_cm`, `product_width_cm`

### Insights:
- **Product Detail Impact:** Evaluate if detailed product descriptions or more photos lead to higher sales or better customer satisfaction.
- **Shipping Cost Correlation:** Assess whether product weight/size influences shipping costs and its correlation with customer satisfaction or purchase decisions.
