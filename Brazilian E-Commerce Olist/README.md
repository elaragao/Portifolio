# Brazilian E-Commerce Public Dataset by Olist


## 1 – Project description
This is a Brazilian ecommerce public dataset of orders made at Olist Store. The dataset has information of 100k orders from 2016 to 2018 made at multiple marketplaces in Brazil. Its features allows viewing an order from multiple dimensions: from order status, price, payment and freight performance to customer location, product attributes and finally reviews written by customers. We also released a geolocation dataset that relates Brazilian zip codes to lat/lng coordinates.


## 2 – Business Problem and Objectives

## 3 – Database Description



[Link to dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce/data)


![Alt text](images/image_dataset.png)


- `olist_customers_dataset`:
  - :key:**customer_id**: key to the orders dataset. Each order has a unique customer_id.
  - :key:**customer_unique_id**: unique identifier of a customer.
  - **customer_zip_code_prefix**: first five digits of customer zip code
  - **customer_city**: customer city name
  - **customer_state**: customer state


- `olist_geolocation_dataset`:
  - **geolocation_zip_code_prefix**: first 5 digits of zip code
  - **geolocation_lat**: latitude
  - **geolocation_lng**: longitude
  - **geolocation_city**: city name
  - **geolocation_state**: state


- `olist_order_items_dataset`:
  - :key:**order_id**: order unique identifier
  - :key:**order_item_id**: sequential number identifying number of items included in the same order.
  - :key:**product_id**: product unique identifier
  - :key:**seller_id**: seller unique identifier
  - **shipping_limit_date**: Shows the seller shipping limit date for handling the order over to the logistic partner.
  - **price**: item price
  - **freight_value**: item freight value item (if an order has more than one item the freight value is splitted between items)


- `olist_order_payments_dataset`:
  - :key:**order_id**: unique identifier of an order.
  - **payment_sequential**: a customer may pay an order with more than one payment method. If he does so, a sequence will be created to accommodate all payments.
  - **payment_type**: method of payment chosen by the customer.
  - **payment_installments**: number of installments chosen by the customer.
  - **payment_value**: transaction value.


- `olist_order_reviews_dataset`:
  - :key:**review_id**: unique review identifier
  - :key:**order_id**: unique order identifier
  - **review_score**: Note ranging from 1 to 5 given by the customer on a satisfaction survey.
  - **review_comment_title**: Comment title from the review left by the customer, in Portuguese.
  - **review_comment_message**: Comment message from the review left by the customer, in Portuguese.
  - **review_creation_date**: Shows the date in which the satisfaction survey was sent to the customer.
  - **review_answer_timestamp**: Shows satisfaction survey answer timestamp.


- `olist_orders_dataset`:
  - :key:**order_id**: unique identifier of the order.
  - :key:**customer_id**: key to the customer dataset. Each order has a unique customer_id.
  - **order_status**: Reference to the order status (delivered, shipped, etc).
  - **order_purchase_timestamp**: Shows the purchase timestamp.
  - **order_approved_at**: Shows the payment approval timestamp.
  - **order_delivered_carrier_date**: Shows the order posting timestamp. When it was handled to the logistic partner.
  - **order_delivered_customer_date**: Shows the actual order delivery date to the customer.
  - **order_estimated_delivery_date**: Shows the estimated delivery date that was informed to customer at the purchase moment.


- `olist_products_dataset`:
  - :key:**product_id**: unique product identifier
  - **product_category_name**: root category of product, in Portuguese.
  - **product_name_lenght**: number of characters extracted from the product name.
  - **product_description_lenght**: number of characters extracted from the product description.
  - **product_photos_qty**: number of product published photos
  - **product_weight_g**: product weight measured in grams.
  - **product_length_cm**: product length measured in centimeters.
  - **product_height_cm**: product height measured in centimeters.
  - **product_width_cm**: product width measured in centimeters.


- `olist_sellers_dataset.csv`:
  - :key:**seller_id**: seller unique identifier
  - **seller_zip_code_prefix**: first 5 digits of seller zip code
  - **seller_city**: seller city name
  - **seller_state**: seller state

    
- `product_category_name_translation`:
  - **product_category_name**: category name in Portuguese
  - **product_category_name_english**: category name in English



## 4 – Solution pipeline
## 5 – Technologies and tools

## 6 – Project Structure

