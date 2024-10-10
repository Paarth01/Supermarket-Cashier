# Python Billing System

This Python script is designed to simulate a simple billing system for a store, allowing users to input products, calculate prices, and apply membership-based discounts.

## Table of Contents
- [Features](#features)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Requirements](#requirements)

---

## Features

1. **Product Entry**: Allows the user to enter products and their quantities.
2. **Price Calculation**: Computes the total price based on predefined product prices.
3. **Discount Calculation**: Applies a discount based on membership type (Gold, Silver, Bronze) for bills over $25.
4. **Final Bill Display**: Displays the total discounted price.

---

## Usage

1. **Run the Script**: Execute the script, and follow the prompts.
2. **Enter Products**: 
   - Press `A` to add a product.
   - Input the product name and its quantity.
   - Press `Q` to finish entering products.
3. **Enter Membership**: Choose from `Gold`, `Silver`, `Bronze` membership options.
4. **View Bill**: The script will display each product's price, calculate the subtotal, apply any discount, and show the final bill amount.

---

## Code Explanation

1. **`enterProducts()`**: 
   - This function collects product names and quantities from the user.
   - It stores the data in a dictionary (`buyingData`), where the product is the key and the quantity is the value.

2. **`getPrice(product, quantity)`**:
   - Takes a product and its quantity as input.
   - Retrieves the price from a predefined dictionary (`priceData`) and calculates the subtotal for that product.
   - Prints the calculation in a format like `Product: $Price x Quantity = Subtotal`.

3. **`getDiscount(billAmount, membership)`**:
   - Calculates a discount based on the total bill amount and membership type.
   - Gold: 20% discount, Silver: 10%, Bronze: 5%, applicable only if the bill is $25 or more.
   - Prints the discounted price.

4. **`makeBill(buyingData, membership)`**:
   - Combines the product prices and applies any applicable discounts.
   - Displays the final bill.

5. **Execution Flow**:
   - The script starts by calling `enterProducts()` to gather product data.
   - After the user inputs the membership type, `makeBill()` processes the prices and discounts, and displays the final total.

---
