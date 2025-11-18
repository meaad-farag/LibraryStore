

# MIAD Book Store: E-Commerce Web Application

##  Project Overview

**MIAD Book Store** is a fully integrated e-commerce system designed to simulate a functional online bookstore. [cite\_start]This project demonstrates full-stack development proficiency by implementing distinct user and administrative interfaces for seamless product management, shopping, and order processing[cite: 3].

This application serves as a practical showcase of my skills in web development using the standard XAMPP environment.

[cite\_start]**Developed by:** Meaad Farag [cite: 1]
[cite\_start]**ID:** 190706821 [cite: 2]

##  Technologies Used

| Category | Technology | Role in Project |
| :--- | :--- | :--- |
| **Languages** | HTML, CSS, PHP, SQL | [cite\_start]Core languages for building the UI, server-side logic, and database interaction[cite: 232]. |
| **Database** | MySQL / MariaDB | [cite\_start]Used for storing and managing data related to users, products, and orders[cite: 232]. |
| **Environment** | XAMPP (Apache Web Server) | Local server environment to run PHP scripts and provide database access. |

##  Key Features and Functionality

The project implements a complete system for both customer interaction and administrative control.

###  User Interface & Functions

  * [cite\_start]**Product Browsing:** Users can view all available books or filter products by category (e.g., Children's Books, Novels)[cite: 9, 10, 19, 20].
  * [cite\_start]**Shopping Cart:** Users can add products to the cart, view cart contents, manage quantities, and delete items[cite: 7, 13, 29].
  * [cite\_start]**Checkout Process:** Dedicated pages for filling in shipping and payment information to complete the purchase[cite: 8, 21].
  * [cite\_start]**Authentication:** Includes dedicated pages for user registration and login[cite: 14, 24].

###  Admin Control Panel (CRUD Operations)

  * [cite\_start]**Product Management:** Administrators can add new products [cite: 14][cite\_start], update product details [cite: 27][cite\_start], and delete products from the site[cite: 12].
  * [cite\_start]**Order Tracking:** Displays data of completed orders and invoices for administrative review[cite: 30].
  * [cite\_start]**Admin Authentication:** Separate pages for administrator registration and login to access the control panel[cite: 5, 6].

##  Local Deployment Guide (XAMPP Setup)

To run this project locally, ensure you have XAMPP installed and follow these steps:

### 1\. Configure the Server Environment

  * **Start XAMPP:** Launch the XAMPP Control Panel and ensure both **Apache** and **MySQL** modules are running (indicated by a green status).

### 2\. Place Project Files

  * **Copy Project:** Copy the entire project folder (**`e-commerce`**) and place it into the XAMPP web root directory:
    ```
    C:\xampp\htdocs\
    ```

### 3\. Database Setup (Import Schema)

The database schema and initial data are provided in the **`book-store.sql`** file.

  * **Open phpMyAdmin:** Navigate to `http://localhost/phpmyadmin/`.
  * **Create Database:** Create a new database named **`book-store`** (must be exact).
  * **Import File:** Select the newly created `book-store` database, go to the **Import** tab, and upload the **`book-store.sql`** file. This will create all necessary tables (like `admin_users`, `products`, etc.) and populate them with initial data.

### 4\. Access the Application

Once the database import is complete, access the application via your web browser:

```
http://localhost/e-commerce/
```

**Default Admin Login:** Please refer to the initial `INSERT` statement in the `book-store.sql` file for the default administrator credentials.

##  Key Project Files

| File Name | Functional Description |
| :--- | :--- |
| [cite\_start]`config.php` [cite: 11] | Handles the database connection parameters. |
| [cite\_start]`index.php` [cite: 14] | Primary Admin Panel interface to add products. |
| [cite\_start]`products.php` [cite: 23] | Displays all products on the admin page for modification and deletion. |
| [cite\_start]`orders.php` [cite: 30] | Displays completed order data and invoices to the admin. |
| [cite\_start]`session_shop.php` [cite: 25] | Home page view for logged-in users. |
| [cite\_start]`checkout.php` [cite: 8] | Handles the collection of shipping and payment information. |
| [cite\_start]`pay_confirm.php` [cite: 21] | Confirms the purchase completion and saves the order data in the database. |
