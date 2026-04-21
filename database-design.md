# Database Design

## Tables

### users
- id
- username
- email
- password
- created_at

### products
- id
- name
- description
- price
- stock
- created_at

### cart_items
- id
- user_id
- product_id
- quantity
- created_at

### orders
- id
- user_id
- status
- created_at

### order_items
- id
- order_id
- product_id
- quantity
- price_at_purchase

## Relationships
- A user has many cart_items
- A product has many cart_items
- A user has many orders
- An order has many order_items
- A product has many order_items