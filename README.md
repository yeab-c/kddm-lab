# Short Note

## A. Two columns in the customers table look like customer identifiers. How do they differ, and which one would you use to count customers?

- customer_id has 99441 distinct values out of 99441 rows, so it is the primary key, but it only identifies one order. customer_unique_id has 96096 distinct values, because the same person gets a new customer_id everytime they place an order. So i would use customer_unique_id to count customers.



## B. Which table is a junction table, and which relationships does it resolve?

- order_items is the junction table. It connects orders, products and sellers, so it resolves the many to many between orders and products, and between orders and sellers.



## C. Name one relationship where the data is stricter than your diagram, and one where the circle on your diagram is justified by the data

- The customers to orders relationship is stricter than my diagram. I drew zero or many orders per customer_id, but the data shows exactly one order for each customer_id. The circle between orders and order_items is justified, because 775 orders have no items.