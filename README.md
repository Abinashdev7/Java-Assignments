Campus Cafe Inventory – Java Assignment

Project Overview

This project is a menu-driven Java application that manages product inventory for a campus cafe. It allows users to add products, display available products, calculate total stock value and average price, restock existing products, and duplicate products using a copy constructor.

Files Included

Product.java – Defines the Product class with product name, price, quantity, static totalProducts, copy constructor, stockValue(), and display() methods.

Main.java – Contains the menu-driven application and handles product operations, restocking, duplication, and user input.

Warmup.java – Demonstrates Java concepts such as object creation, static variables, instance variables, arithmetic operations, and type casting.

output.txt – Contains the console output from the complete application test session.


Assignment Questions:

1. What did you predict for Warmup.java, and what did it actually print? Explain the lines that surprised you.

I expected Warmup.java to demonstrate product creation, stock value calculation, average price calculation, and the total number of products created. The output demonstrated that the copy constructor creates another Product object and increments the static counter, while converting a double to an integer removes its decimal portion instead of rounding it.

2. What is the difference between the static variable totalProducts and the instance variable name?

The totalProducts variable is static, meaning it is shared among all Product objects and maintains a common count of products created. The name variable is an instance variable, meaning every Product object maintains its own product name independently.

3. What does the copy constructor do, and why does changing p2.name not change p1.name?

The copy constructor creates a new Product object by copying the name, price, and quantity from an existing Product object. Since p1 and p2 are separate objects with their own instance variables, changing the name of p2 does not affect the name of p1.

4. Why does Java force you to write (int) average when converting a double to an int, and what happens to the decimal part?

Java requires an explicit cast because converting a double to an int is a narrowing conversion that may result in loss of information. When (int) average is used, Java discards the decimal portion without rounding, so 10249.5 becomes 10249.