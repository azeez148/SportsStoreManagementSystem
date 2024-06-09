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
