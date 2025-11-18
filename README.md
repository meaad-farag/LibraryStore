
# MIAD Book Store: E-Commerce Web Application

## Project Overview

**MIAD Book Store** is a fully integrated e-commerce system designed to simulate a functional online bookstore.
This project demonstrates full-stack development proficiency by implementing distinct user and administrative interfaces for seamless product management, shopping, and order processing.

This application serves as a practical showcase of my skills in web development using the standard XAMPP environment.

**Developed by:** Meaad Farag

## Technologies Used

| Category        | Technology                | Role in Project                                                                  |
| :-------------- | :------------------------ | :------------------------------------------------------------------------------- |
| **Languages**   | HTML, CSS, PHP, SQL       | Core languages for building the UI, server-side logic, and database interaction. |
| **Database**    | MySQL / MariaDB           | Used for storing and managing data related to users, products, and orders.       |
| **Environment** | XAMPP (Apache Web Server) | Local server environment to run PHP scripts and provide database access.         |

## Key Features and Functionality

The project implements a complete system for both customer interaction and administrative control.

### User Interface & Functions

* **Product Browsing:** Users can view all available books or filter products by category (e.g., Children's Books, Novels).
* **Shopping Cart:** Users can add products to the cart, view cart contents, manage quantities, and delete items.
* **Checkout Process:** Dedicated pages for filling in shipping and payment information to complete the purchase.
* **Authentication:** Includes dedicated pages for user registration and login.

### Admin Control Panel (CRUD Operations)

* **Product Management:** Administrators can add new products, update product details, and delete products from the site.
* **Order Tracking:** Displays data of completed orders and invoices for administrative review.
* **Admin Authentication:** Separate pages for administrator registration and login to access the control panel.

## Local Deployment Guide (XAMPP Setup)

To run this project locally, ensure you have XAMPP installed and follow these steps:

### 1. Configure the Server Environment

* **Start XAMPP:** Launch the XAMPP Control Panel and ensure both **Apache** and **MySQL** modules are running (indicated by a green status).

### 2. Place Project Files

* **Copy Project:** Copy the entire project folder (**`e-commerce`**) and place it into the XAMPP web root directory:

  ```
  C:\xampp\htdocs\
  ```

### 3. Database Setup (Import Schema)

The database schema and initial data are provided in the **`book-store.sql`** file.

* **Open phpMyAdmin:** Navigate to `http://localhost/phpmyadmin/`.
* **Create Database:** Create a new database named **`book-store`** (must be exact).
* **Import File:** Select the newly created `book-store` database, go to the **Import** tab, and upload the **`book-store.sql`** file. This will create all necessary tables (like `admin_users`, `products`, etc.) and populate them with initial data.

### 4. Access the Application

Once the database import is complete, access the application via your web browser:

```
http://localhost/e-commerce/
```

**Default Admin Login:** Please refer to the initial `INSERT` statement in the `book-store.sql` file for the default administrator credentials, or register as a new admin and log in using the new username and password.

## Key Project Files

| File Name          | Functional Description                                                     |
| :----------------- | :------------------------------------------------------------------------- |
| `config.php`       | Handles the database connection parameters.                                |
| `index.php`        | Primary Admin Panel interface to add products.                             |
| `products.php`     | Displays all products on the admin page for modification and deletion.     |
| `orders.php`       | Displays completed order data and invoices to the admin.                   |
| `session_shop.php` | Home page view for logged-in users.                                        |
| `checkout.php`     | Handles the collection of shipping and payment information.                |
| `pay_confirm.php`  | Confirms the purchase completion and saves the order data in the database. |

---

