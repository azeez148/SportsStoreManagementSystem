# SportsStoreManagementSystem
SportsStoreManagementSystem

### Initial Plan and Requirement Document for Sportswear, Footwear, and Sports Accessories Management Application

#### 1. **Introduction**

This document outlines the initial plan and requirements for a sportswear, footwear, and sports accessories management application. The application will facilitate operations for three types of users: Admin, Staff, and Customers, with each having specific functionalities.

#### 2. **Tech Stack**

- **Frontend:** Angular 17 or 18
- **Backend:** Spring Boot
- **Database:** MySQL or PostgreSQL
- **Cloud Services:** AWS tools (if useful)

#### 3. **User Roles and Functionalities**

##### 3.1 Admin Functionalities

- **CRUD Operations on Shops**
  - Create, Read, Update, Delete shops.
- **CRUD Operations on Staff and Customers**
  - Create, Read, Update, Delete staff members and customers.
- **CRUD Operations on Product Categories**
  - Create, Read, Update, Delete product categories.
- **CRUD Operations on Products**
  - Create, Read, Update, Delete products.
- **CRUD Operations on Sales**
  - Create, Read, Update, Delete sales records.
- **CRUD Operations on Purchases**
  - Create, Read, Update, Delete purchase records.
- **CRUD Operations on Invoices**
  - Create, Read, Update, Delete invoices.
- **CRUD Operations on Reports**
  - Generate and manage various reports.
- **Profile Management**
  - Update personal profile information.
- **Password Management**
  - Reset password functionality.
- **Session Management**
  - Logout from the system.

##### 3.2 Staff Functionalities

- **CRUD Operations on Customers**
  - Create, Read, Update, Delete customer information.
- **CRUD Operations on Product Categories**
  - Create, Read, Update, Delete product categories.
- **CRUD Operations on Products**
  - Create, Read, Update, Delete products.
- **CRUD Operations on Sales**
  - Create, Read, Update, Delete sales records.
- **CRUD Operations on Purchases**
  - Create, Read, Update, Delete purchase records.
- **CRUD Operations on Invoices**
  - Create, Read, Update, Delete invoices.
- **CRUD Operations on Reports**
  - Generate and manage various reports.
- **Profile Management**
  - Update personal profile information.
- **Password Management**
  - Reset password functionality.
- **Session Management**
  - Logout from the system.

##### 3.3 Customer Functionalities

- **List Operations on Shops**
  - View list of shops.
- **List Operations on Product Categories**
  - View list of product categories.
- **List Operations on Products**
  - View list of products.
- **Sales Operations**
  - Create and update sales records.
- **List Operations on Invoices**
  - View invoices.
- **Profile Management**
  - Update personal profile information.
- **Password Management**
  - Reset password functionality.
- **Session Management**
  - Logout from the system.

#### 4. **High-Level Architecture**

1. **Frontend (Angular)**
   - Develop a responsive and user-friendly UI.
   - Components for each user role (Admin, Staff, Customer).
   - Use Angular services for API calls.

2. **Backend (Spring Boot)**
   - Implement RESTful APIs for CRUD operations.
   - Implement security for role-based access control.
   - Use Spring Data JPA for database interactions.
   - Use Spring Security for authentication and authorization.

3. **Database (MySQL/PostgreSQL)**
   - Design schema for shops, users (staff and customers), product categories, products, sales, purchases, invoices, and reports.
   - Use relational design principles to ensure data integrity and efficiency.

4. **Cloud Services (AWS)**
   - Use AWS RDS for database management (if needed).
   - Use AWS S3 for storing files and images (if needed).
   - Use AWS Lambda for serverless functions (if needed).
   - Use AWS Cognito for user authentication (if needed).

#### 5. **Initial Development Plan**

1. **Requirement Gathering**
   - Finalize requirements and create detailed user stories.

2. **Design Phase**
   - Create wireframes for the application.
   - Design database schema.
   - Define API endpoints and data contracts.

3. **Setup Development Environment**
   - Configure Angular, Spring Boot, and database environment.
   - Setup version control with Git.

4. **Development Phase**
   - **Week 1-2:** Implement authentication and authorization.
   - **Week 3-4:** Develop CRUD operations for shops, users, and product categories.
   - **Week 5-6:** Implement CRUD operations for products, sales, and purchases.
   - **Week 7-8:** Implement invoice management and reporting features.
   - **Week 9-10:** Develop frontend components for all functionalities.
   - **Week 11-12:** Integrate frontend with backend APIs.

5. **Testing Phase**
   - Unit testing for backend and frontend.
   - Integration testing for API endpoints.
   - User acceptance testing (UAT).

6. **Deployment Phase**
   - Configure CI/CD pipeline.
   - Deploy the application on AWS.

7. **Post-Deployment**
   - Monitor application performance.
   - Collect user feedback and iterate on improvements.

#### 6. **Requirement Document**

##### 6.1 Functional Requirements

- **User Authentication**
  - Users should be able to register, login, and reset passwords.
  - Role-based access control for Admin, Staff, and Customer.

- **Shop Management**
  - Admin should be able to perform CRUD operations on shops.

- **User Management**
  - Admin and Staff should be able to manage customer information.
  - Admin should be able to manage staff information.

- **Product Management**
  - Admin and Staff should be able to manage product categories and products.

- **Sales Management**
  - Admin and Staff should be able to manage sales records.
  - Customers should be able to create and update sales.

- **Purchases Management**
  - Admin and Staff should be able to manage purchase records.

- **Invoice Management**
  - Admin and Staff should be able to manage invoices.
  - Customers should be able to view invoices.

- **Reporting**
  - Admin and Staff should be able to generate and view reports.

- **Profile Management**
  - All users should be able to update their profile information.

- **Password Management**
  - All users should be able to reset their passwords.

- **Session Management**
  - All users should be able to logout from the system.

##### 6.2 Non-Functional Requirements

- **Performance**
  - The system should be able to handle up to 10,000 concurrent users.
- **Scalability**
  - The system should be easily scalable to accommodate future growth.
- **Security**
  - The system should implement best practices for data security and user privacy.
- **Usability**
  - The UI should be intuitive and easy to navigate.
- **Maintainability**
  - The codebase should be well-documented and modular to facilitate maintenance.


WireFrame:
Creating wireframes is an essential step in the design phase of the application development process. Below are the wireframes for the main screens and functionalities for Admin, Staff, and Customer roles in the sportswear, footwear, and sports accessories management application.

### Wireframes

#### 1. **Login Page**
   - Fields: Username, Password
   - Buttons: Login, Forgot Password, Register

```
-------------------------------------
|          Sports Management        |
-------------------------------------
| Username: [_____________________] |
| Password: [_____________________] |
|                                   |
| [ Login ]       [ Forgot Password ]|
|                                   |
| [ Register ]                      |
-------------------------------------
```

#### 2. **Admin Dashboard**
   - Navigation: Shops, Staff, Customers, Product Categories, Products, Sales, Purchases, Invoices, Reports, Profile, Logout
   - Main Area: Overview of key metrics (Total Sales, Total Purchases, Number of Shops, etc.)

```
-------------------------------------
| Sports Management - Admin Dashboard |
-------------------------------------
| Home | Shops | Staff | Customers  | 
| Product Categories | Products     | 
| Sales | Purchases | Invoices      |
| Reports | Profile | Logout        |
-------------------------------------
|       Key Metrics                  |
|  -------------------------------   |
| | Total Sales:          $xxxxx |   |
| | Total Purchases:      $xxxxx |   |
| | Number of Shops:      xx     |   |
| | Number of Products:   xxx    |   |
|  -------------------------------   |
-------------------------------------
```

#### 3. **Shop Management (Admin)**
   - Table: List of Shops (Name, Location, Manager)
   - Buttons: Add Shop, Edit, Delete

```
-------------------------------------
| Sports Management - Shops         |
-------------------------------------
| [ Add Shop ]                      |
|-----------------------------------|
| Shop Name  | Location  | Manager  |
|-----------------------------------|
| Shop 1     | Location 1| Manager 1|
| Shop 2     | Location 2| Manager 2|
| ...                                |
|-----------------------------------|
| [ Edit ] [ Delete ]               |
-------------------------------------
```

#### 4. **Staff Management (Admin)**
   - Table: List of Staff (Name, Role, Email)
   - Buttons: Add Staff, Edit, Delete

```
-------------------------------------
| Sports Management - Staff         |
-------------------------------------
| [ Add Staff ]                     |
|-----------------------------------|
| Staff Name | Role  | Email        |
|-----------------------------------|
| Staff 1    | Role 1| email1@...   |
| Staff 2    | Role 2| email2@...   |
| ...                                |
|-----------------------------------|
| [ Edit ] [ Delete ]               |
-------------------------------------
```

#### 5. **Customer Management (Admin/Staff)**
   - Table: List of Customers (Name, Email, Phone)
   - Buttons: Add Customer, Edit, Delete

```
-------------------------------------
| Sports Management - Customers     |
-------------------------------------
| [ Add Customer ]                  |
|-----------------------------------|
| Customer Name | Email   | Phone   |
|-----------------------------------|
| Customer 1    | email1@ | 12345678|
| Customer 2    | email2@ | 87654321|
| ...                                |
|-----------------------------------|
| [ Edit ] [ Delete ]               |
-------------------------------------
```

#### 6. **Product Categories Management (Admin/Staff)**
   - Table: List of Categories (Name, Description)
   - Buttons: Add Category, Edit, Delete

```
-------------------------------------
| Sports Management - Categories    |
-------------------------------------
| [ Add Category ]                  |
|-----------------------------------|
| Category Name | Description       |
|-----------------------------------|
| Category 1    | Desc 1            |
| Category 2    | Desc 2            |
| ...                                |
|-----------------------------------|
| [ Edit ] [ Delete ]               |
-------------------------------------
```

#### 7. **Products Management (Admin/Staff)**
   - Table: List of Products (Name, Category, Price, Stock)
   - Buttons: Add Product, Edit, Delete

```
-------------------------------------
| Sports Management - Products      |
-------------------------------------
| [ Add Product ]                   |
|-----------------------------------|
| Product Name | Category | Price   | Stock |
|-------------------------------------------|
| Product 1    | Cat 1    | $xxx    | xx    |
| Product 2    | Cat 2    | $yyy    | yy    |
| ...                                |
|-------------------------------------------|
| [ Edit ] [ Delete ]               |
-------------------------------------
```

#### 8. **Sales Management (Admin/Staff/Customer)**
   - Table: List of Sales (Product, Quantity, Price, Date)
   - Buttons: Add Sale, Edit, Delete (for Admin/Staff), Create Sale (for Customer)

```
-------------------------------------
| Sports Management - Sales         |
-------------------------------------
| [ Add Sale ]                      | [ Create Sale ] (Customer)
|-----------------------------------|
| Product   | Quantity | Price | Date |
|-------------------------------------|
| Product 1 | 10       | $xxx  | xx/xx|
| Product 2 | 5        | $yyy  | yy/yy|
| ...                                |
|-------------------------------------|
| [ Edit ] [ Delete ]               |
-------------------------------------
```

#### 9. **Purchases Management (Admin/Staff)**
   - Table: List of Purchases (Product, Quantity, Price, Date)
   - Buttons: Add Purchase, Edit, Delete

```
-------------------------------------
| Sports Management - Purchases     |
-------------------------------------
| [ Add Purchase ]                  |
|-----------------------------------|
| Product   | Quantity | Price | Date |
|-------------------------------------|
| Product 1 | 100      | $xxxx | xx/xx|
| Product 2 | 50       | $yyyy | yy/yy|
| ...                                |
|-------------------------------------|
| [ Edit ] [ Delete ]               |
-------------------------------------
```

#### 10. **Invoices Management (Admin/Staff/Customer)**
   - Table: List of Invoices (Invoice Number, Customer, Date, Total Amount)
   - Buttons: Add Invoice, Edit, Delete (for Admin/Staff), View Invoice (for Customer)

```
-------------------------------------
| Sports Management - Invoices      |
-------------------------------------
| [ Add Invoice ]                   |
|-----------------------------------|
| Invoice #  | Customer   | Date | Total  |
|------------------------------------------|
| 12345      | Customer 1 | xx/xx| $xxx   |
| 12346      | Customer 2 | yy/yy| $yyy   |
| ...                                |
|------------------------------------------|
| [ Edit ] [ Delete ]     [ View ]        |
-------------------------------------
```

#### 11. **Reports (Admin/Staff)**
   - Options: Generate Sales Report, Generate Purchase Report, Generate Inventory Report
   - Date Range Selection
   - Generate Report Button

```
-------------------------------------
| Sports Management - Reports       |
-------------------------------------
| [Generate Sales Report]           |
| [Generate Purchase Report]        |
| [Generate Inventory Report]       |
|-----------------------------------|
| Select Date Range:                |
| From: [xx/xx/xxxx] To: [yy/yy/yyyy]|
|-----------------------------------|
| [ Generate Report ]               |
-------------------------------------
```

#### 12. **Profile Management (Admin/Staff/Customer)**
   - Fields: Name, Email, Phone, Address
   - Buttons: Update Profile, Change Password

```
-------------------------------------
| Sports Management - Profile       |
-------------------------------------
| Name:    [_____________________]  |
| Email:   [_____________________]  |
| Phone:   [_____________________]  |
| Address: [_____________________]  |
|                                   |
| [ Update Profile ] [ Change Password ] |
-------------------------------------
```

These wireframes provide a visual guide for the application's main screens and functionalities, ensuring a consistent and user-friendly interface for all roles. The detailed design can be further refined based on user feedback and additional requirements during the development process.


Database Schema Design:

Designing the database schema is crucial to ensure data integrity, efficiency, and scalability. Below is the database schema for the sportswear, footwear, and sports accessories management application. The schema includes tables for users, shops, product categories, products, sales, purchases, invoices, and reports.

### Database Schema

#### 1. **Users Table**
   - **Columns:**
     - `user_id` (Primary Key)
     - `username` (Unique)
     - `password`
     - `email` (Unique)
     - `phone`
     - `address`
     - `role` (ENUM: 'Admin', 'Staff', 'Customer')
     - `created_at`
     - `updated_at`

```sql
CREATE TABLE users (
    user_id SERIAL PRIMARY KEY,
    username VARCHAR(50) UNIQUE NOT NULL,
    password VARCHAR(255) NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    phone VARCHAR(20),
    address TEXT,
    role ENUM('Admin', 'Staff', 'Customer') NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
);
```

#### 2. **Shops Table**
   - **Columns:**
     - `shop_id` (Primary Key)
     - `name`
     - `location`
     - `manager_id` (Foreign Key references `users.user_id`)
     - `created_at`
     - `updated_at`

```sql
CREATE TABLE shops (
    shop_id SERIAL PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    location TEXT NOT NULL,
    manager_id INT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    FOREIGN KEY (manager_id) REFERENCES users(user_id)
);
```

#### 3. **Product Categories Table**
   - **Columns:**
     - `category_id` (Primary Key)
     - `name`
     - `description`
     - `created_at`
     - `updated_at`

```sql
CREATE TABLE product_categories (
    category_id SERIAL PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    description TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
);
```

#### 4. **Products Table**
   - **Columns:**
     - `product_id` (Primary Key)
     - `name`
     - `category_id` (Foreign Key references `product_categories.category_id`)
     - `price`
     - `stock`
     - `shop_id` (Foreign Key references `shops.shop_id`)
     - `created_at`
     - `updated_at`

```sql
CREATE TABLE products (
    product_id SERIAL PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    category_id INT,
    price DECIMAL(10, 2) NOT NULL,
    stock INT NOT NULL,
    shop_id INT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    FOREIGN KEY (category_id) REFERENCES product_categories(category_id),
    FOREIGN KEY (shop_id) REFERENCES shops(shop_id)
);
```

#### 5. **Sales Table**
   - **Columns:**
     - `sale_id` (Primary Key)
     - `product_id` (Foreign Key references `products.product_id`)
     - `customer_id` (Foreign Key references `users.user_id`)
     - `quantity`
     - `total_price`
     - `sale_date`
     - `created_at`
     - `updated_at`

```sql
CREATE TABLE sales (
    sale_id SERIAL PRIMARY KEY,
    product_id INT,
    customer_id INT,
    quantity INT NOT NULL,
    total_price DECIMAL(10, 2) NOT NULL,
    sale_date TIMESTAMP NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    FOREIGN KEY (product_id) REFERENCES products(product_id),
    FOREIGN KEY (customer_id) REFERENCES users(user_id)
);
```

#### 6. **Purchases Table**
   - **Columns:**
     - `purchase_id` (Primary Key)
     - `product_id` (Foreign Key references `products.product_id`)
     - `quantity`
     - `total_price`
     - `purchase_date`
     - `created_at`
     - `updated_at`

```sql
CREATE TABLE purchases (
    purchase_id SERIAL PRIMARY KEY,
    product_id INT,
    quantity INT NOT NULL,
    total_price DECIMAL(10, 2) NOT NULL,
    purchase_date TIMESTAMP NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    FOREIGN KEY (product_id) REFERENCES products(product_id)
);
```

#### 7. **Invoices Table**
   - **Columns:**
     - `invoice_id` (Primary Key)
     - `sale_id` (Foreign Key references `sales.sale_id`)
     - `customer_id` (Foreign Key references `users.user_id`)
     - `total_amount`
     - `invoice_date`
     - `created_at`
     - `updated_at`

```sql
CREATE TABLE invoices (
    invoice_id SERIAL PRIMARY KEY,
    sale_id INT,
    customer_id INT,
    total_amount DECIMAL(10, 2) NOT NULL,
    invoice_date TIMESTAMP NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
    FOREIGN KEY (sale_id) REFERENCES sales(sale_id),
    FOREIGN KEY (customer_id) REFERENCES users(user_id)
);
```

#### 8. **Reports Table**
   - **Columns:**
     - `report_id` (Primary Key)
     - `report_type` (ENUM: 'Sales', 'Purchases', 'Inventory')
     - `generated_by` (Foreign Key references `users.user_id`)
     - `date_range_start`
     - `date_range_end`
     - `created_at`

```sql
CREATE TABLE reports (
    report_id SERIAL PRIMARY KEY,
    report_type ENUM('Sales', 'Purchases', 'Inventory') NOT NULL,
    generated_by INT,
    date_range_start TIMESTAMP NOT NULL,
    date_range_end TIMESTAMP NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    FOREIGN KEY (generated_by) REFERENCES users(user_id)
);
```

### Entity-Relationship Diagram (ERD)

```plaintext
+------------+       +-------------+        +--------------------+      +---------------+
|    users   |       |    shops    |        | product_categories |      |    products   |
+------------+       +-------------+        +--------------------+      +---------------+
| user_id PK |<----->| shop_id PK  |<-----+ | category_id PK     |<--+  | product_id PK |
| username   |       | name        |      | | name               |   |  | name          |
| password   |       | location    |      | | description        |   |  | category_id FK|
| email      |       | manager_id FK|      | +--------------------+   |  | price         |
| phone      |       | created_at  |      |                           |  | stock         |
| address    |       | updated_at  |      |                           |  | shop_id FK    |
| role       |       +-------------+      |                           |  | created_at    |
| created_at |                               |                           |  | updated_at    |
| updated_at |                               |                           +---------------+
+------------+                               |                            
                                            |        +-------------+
+--------------+   +-----------+             |        |  purchases |
|    sales     |   | invoices  |             |        +-------------+
+--------------+   +-----------+             |        | purchase_id PK|
| sale_id PK   |<->| invoice_id |             |        | product_id FK |
| product_id FK|   | sale_id FK |             |        | quantity      |
| customer_id FK|  | customer_id FK|             |        | total_price  |
| quantity     |   | total_amount|             |        | purchase_date |
| total_price  |   | invoice_date|             |        | created_at    |
| sale_date    |   | created_at |             |        | updated_at    |
| created_at   |   | updated_at |             |        +-------------+
| updated_at   |   +-----------+             |
+--------------+                             |
                                            | 
                                            +------------------+
                                            |      reports     |
                                            +------------------+
                                            | report_id PK     |
                                            | report_type      |
                                            | generated_by FK  |
                                            | date_range_start |
                                            | date_range_end   |
                                            | created_at       |
                                            +------------------+
```

### Summary
- **Users Table:** Manages user information including roles (Admin, Staff, Customer).
- **Shops Table:** Manages shop details and links to shop managers.
- **Product Categories Table:** Manages categories for products.
- **Products Table:** Manages products linked to categories and shops.
- **Sales Table:** Manages sales records linked to products and customers.
- **Purchases Table:** Manages purchase records linked to products.
- **Invoices Table:** Manages invoices linked to sales and customers.
- **Reports Table:** Manages generated reports and their details.

This schema ensures that all necessary relationships and data integrity constraints are maintained, facilitating efficient and secure data operations for the application.
