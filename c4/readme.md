# C4 Exercise
Practice selecting appropriate software for a given problem

## Organisation

### Duration

You have **2 hours** to make as much progress on this task as possible.

Make sure to take breaks!

### Team

Pairs of students

## Brief

## Book Haven

A small e-commerce platform called Book Haven is designed to sell books online. The platform allows users to browse, purchase, and review books. 

### C4 Diagram Levels

1. Context Diagram
- Systems in Scope:
  - Book Haven (the e-commerce platform)
  - Users (customers, administrators)
  - Payment Gateway (e.g., PayPal)
  - External Book Suppliers

- Interactions:
  - Users browse and purchase books.
  - Administrators manage inventory and user accounts.
  - Payment Gateway processes transactions.

2. Container Diagram
- Containers:
  - Web Application: User interface for browsing and purchasing books.
  - API Server: Manages requests and responses between the web application and the database.
  - Database: Stores user data, book information, and transaction history.
  - Admin Dashboard: For managing book inventory and user accounts.
- Inter-container interactions:
  - Web Application communicates with the API Server.
  - API Server interacts with the Database and the Admin Dashboard.

3. Component Diagram (for the API Server)
- Components:
  - Authentication Component: Handles user logins and registrations.
  - Book Management Component: Manages book listings and inventory.
  - Order Processing Component: Handles order placements and transactions.
Review System Component: Manages user reviews and ratings.
Interactions:
Authentication Component verifies user identity when accessing sensitive operations.
Order Processing Component interacts with the Payment Gateway to complete transactions.
Code Diagram (for the Book Management Component)
Classes/Modules:
Book: Represents a book object with properties like title, author, and price.
InventoryManager: Manages stock levels and updates the database.
Review: Represents a user review, associated with both a book and a user.
Interactions:
The InventoryManager accesses the Book class when updating stock.
The Review class interacts with both the Book and User classes to link reviews correctly.

## Bonus
- Try and create a diagram of your chosen system using [draw.io](https://app.diagrams.net/) or a tool of your choice
