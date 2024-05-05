# CISC3003-SemesterProject-Part2

# E-Commerce Web Application

## Description
This E-Commerce platform is a fully functional web application developed as part of the CISC3003 course, following the Mr. Web Designer project walkthrough. It allows users to browse products, add them to a shopping cart, and proceed through a checkout process. The platform also includes an administrative interface for managing products and orders.

## Installation

### Prerequisites
- Apache server (XAMPP recommended)
- PHP (version 7.4 or higher)
- MySQL (MariaDB or MySQL proper)

### Setup Instructions

1. **Extract the project:**
   - Extract the project into your web server directory, typically `xampp/htdocs` if you are using XAMPP.

2. **Setting up the environment:**
   - Start the Apache and MySQL modules via the XAMPP control panel.

3. **Database Setup:**
   - Open phpMyAdmin from your XAMPP control panel.
   - Create a new database named `shop_db`.
   - Import the `shop_db.sql` file located in the `CISC3003-SemesterProject-Part2` directory. This file contains all the necessary tables and schema required for the application.

4. **Configuring the Application:**
   - Ensure the `CISC3003-SemesterProject-Part2/project/uploaded_files` directory has appropriate write permissions set, as follows:
  
   ```
     chmod -R 755 /path/to/xampp/htdocs/CISC3003-SemesterProject-Part2/project/uploaded_files/
   ```
      - Adjust the database connection settings if necessary in `CISC3003-SemesterProject-Part2/project/components/connect.php`. Default settings:
  ```
    php
    $dsn = 'mysql:host=localhost;port=3306;dbname=shop_db';
    $username = 'root';
    $password = '';
  ```

5. **Accessing the Project:**
   - Open a web browser and navigate to `localhost/CISC3003-SemesterProject-Part2/project` to access the application.
   - Explore the functionalities like adding products, viewing products, managing the cart, and checking out.


## Features
- **Product Browsing**: View a list of available products.
- **Shopping Cart**: Users can add products to their shopping cart and modify their selections.
- **Checkout Process**: A step-by-step process to complete the purchase.
- **Admin Panel**: Manage products and view orders.

## Additional Notes
- Ensure all dependencies are installed and configured properly as per the prerequisites.
- The platform is designed to run in a local environment for demonstration and development purposes.

## Contact
For any further assistance or queries, please feel free to contact the course instructor or the support team at your institution.
