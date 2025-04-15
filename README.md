# E-commerce System

A simple, object-oriented E-commerce system built using Python. This mini project demonstrates the core functionality of an online shopping platform including product management, cart handling, and order processing.

## Features

- **Product Management**: Create and manage products with name, price, and available stock.
- **Customer Accounts**: Each customer gets a personal shopping cart.
- **Shopping Cart**: Add or remove products, with real-time stock adjustment.
- **Order Processing**: Finalize purchases and calculate total cost.
- **Discount Support**: Option to apply percentage-based discounts.

## Code Structure

- `Product`: Represents a product with attributes like name, price, and stock. Includes logic to update stock.
- `Customer`: Represents a customer who has a shopping cart and can add/remove products.
- `ShoppingCart`: Manages the products in a customer's cart. Supports adding, removing, and applying discounts.
- `Order`: Handles order creation, pricing, and clearing the cart once an order is processed.

## Example Usage

```python
product1 = Product("Laptop", 1000, 5)
product2 = Product("Phone", 500, 10)

customer = Customer("Alice")
customer.add_to_cart(product1, 1)
customer.add_to_cart(product2, 2)

order = Order(customer)
print(order.process_order())
