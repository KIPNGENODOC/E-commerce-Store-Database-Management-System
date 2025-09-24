# E-commerce-Store-Database-Management-System
This system will track:
Customers
Orders
Products
Order Items
Categories
Shipping Information
Payments
**Entities & Relationships Overview**
| Table          | Description                | Relationships                      |
| -------------- | -------------------------- | ---------------------------------- |
| `Customers`    | Stores customer info       | One-to-Many → Orders               |
| `Products`     | Catalog of items for sale  | Many-to-Many → via OrderItems      |
| `Orders`       | Orders placed by customers | One-to-Many → OrderItems, Payments |
| `OrderItems`   | Line items in an order     | Many-to-One → Orders, Products     |
| `Categories`   | Product categories         | One-to-Many → Products             |
| `Payments`     | Payment records            | One-to-One → Orders                |
| `ShippingInfo` | Shipping address per order | One-to-One → Orders                |
