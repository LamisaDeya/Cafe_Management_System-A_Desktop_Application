# Cafe Management System - Java Desktop Application

## Overview
The **Cafe Management System** is a desktop application built using **Java (JFrame)**, **MySQL database**, and **NetBeans IDE**. This system allows cafe managers to handle daily operations efficiently, including managing categories, products, orders, and tracking profits/losses. The application also provides features such as signup/login, inventory management, order placement, and billing.

## Features

### 1. Signup and Login Pages
- Allows new users to register for the system.
- Existing users can log in using their credentials.
- Features a **Forgot Password** page for recovering passwords.

### 2. Product and Category Management
- Admins can add, update, and delete product categories.
- **Add New Product**: Admins can input product details including name, price, category, and upload product images using **JFileChooser**.
- View, edit, and delete existing products.
- Products can be filtered by category and displayed for easy management.

### 3. Inventory Management
- Automatically updates stock levels as products are sold or restocked.
- Displays alerts for products that are out of stock.
- Inventory data is stored in the **MySQL** database and updates in real-time.

### 4. Order Management
- Users can place orders by adding products to a cart.
- The system calculates the total amount for the order.
- A bill is generated with details of the order, including the list of items and prices.
- Admins can verify orders, change their status from **Pending** to **Completed**, and track the order history.

### 5. Billing and Reports
- The system provides a **billing feature** to calculate total sales, capital, expenditure, and profit/loss.
- Admins can generate reports for different periods (daily, monthly, yearly) to track financial performance.
- Detailed profit/loss reports based on overall earnings, capital invested, and expenditures are available.

### 6. Security and Password Management
- Users can change their passwords.
- Security questions are used for additional password recovery options.

### 7. Inventory and Financial Reports
- Admins can view profit/loss reports.
- Earnings and expenses are calculated to show the cafe's financial performance over specific periods.

### 8. Picture Upload for Products
- Admins can upload product images using **JFileChooser**.
- Images are stored locally with a path saved in the **MySQL** database.

## Technologies Used
- **Java (JDK)**: Core logic and desktop application development.
- **JFrame**: Used to build the GUI (Graphical User Interface).
- **MySQL Database**: For data storage including users, products, categories, orders, and financial records.
- **NetBeans IDE**: Integrated development environment used for writing, debugging, and running the application.
- **JDBC (Java Database Connectivity)**: For connecting the application to the **MySQL** database.
- **JFileChooser**: For file uploads (product images).
- **JTable**: Used for displaying data like orders and products in a tabular format.

## Installation and Setup

1. **Install NetBeans IDE**:
   - Download and install **NetBeans IDE** from [NetBeans Official Website](https://netbeans.apache.org/).

2. **Install MySQL Database**:
   - Download and install **MySQL Server** from [MySQL Official Website](https://dev.mysql.com/downloads/installer/).
   - Create a new database named `cafedb`.

3. **Clone the Repository**:
   ```bash
   git clone https://github.com/YourUsername/CafeManagementSystem.git
   ```
4. **Open in NetBeans**:
- Open **NetBeans IDE** and load the project.

5. **Database Setup:**
- Create tables for **Users**, **Categories**, **Products**, **Orders**, **Inventory**, and **Reports** using the provided SQL script in the `db` folder.
- Update the **database connection string** in the code to match your local MySQL settings.

 6. **Run the Application:**
- Run the project from **NetBeans**. The application will connect to the **MySQL** database and launch the GUI.

## Database Structure
- **Users**: Stores user credentials, including usernames, passwords, and security questions.
- **Categories**: Stores product categories.
- **Products**: Stores product information including name, price, category, and image path.
- **Orders**: Stores order details including the list of products, total price, and order status.
- **Inventory**: Tracks product quantities and restocks.
- **Reports**: Stores financial data like earnings, expenses, and profit/loss.

## Key Functionalities

### Admin Features:
- Add, update, or delete categories and products.
- Manage inventory by updating stock as products are sold or restocked.
- View and verify orders.
- Track profits and losses through generated reports.

### User Features:
- Register and log in to the system.
- Place orders and receive generated bills.
- View order history and status.

### Financial Features:
- Generate financial reports for specific periods.
- Track sales, capital, expenditures, and profits.

## Future Improvements
- **Payment Gateway Integration**: Add real-time payment processing for smoother transactions.
- **Enhanced Analytics**: Provide more detailed insights for admins on sales, popular products, and user behavior.
- **Security Enhancements**: Implement two-factor authentication (2FA) for admins and users.
- **Wishlist Feature**: Allow users to add products to a wishlist for future purchases.

## Contributor
- **Lamisa Bintee Mizan Deya**
