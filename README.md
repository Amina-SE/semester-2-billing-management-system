# Billing Management System

A desktop-based Billing Management System developed in **Java** as part of my **Object-Oriented Programming (OOP)** coursework during my 2nd semester at Riphah International University.

The project was initially developed to practice Java and OOP concepts. I later extended the system by integrating **MySQL database connectivity**, improving search and data-management functionality, adding **tooltips**, and implementing **automated PDF invoice generation using iTextPDF**.

---

## Project Overview

The Billing Management System is a Java desktop application designed to manage buyers, products, and billing operations through a graphical user interface.

The system provides separate interfaces for managing buyer and product information and allows users to generate invoices based on billing information.

A major part of the project was also learning how different components work together, including:

- Java
- Object-Oriented Programming
- Java Swing GUI
- MySQL
- JDBC
- iTextPDF
- Event-driven programming
- File generation

The MySQL database integration and additional functionality were incorporated independently to extend the original OOP project.

---

## Main Features

### 1. Login System

The application starts with a login interface that allows the user to access the main system.

---

### 2. Animated Home Page Menu

The home page contains a menu with multiple icons representing different functions of the application.

The menu uses a simple sequential animation:

1. The user clicks the first icon.
2. The first menu item appears.
3. The remaining menu icons then appear one after another.
4. There is approximately a **3–4 second delay** between the appearance of the menu items.
5. This creates a simple animated introduction to the application's main functions.

The menu provides access to features such as:

- Buyer Management
- Product Management
- Billing
- Buyer Details
- Product Details
- Update and Delete Operations
- Logout

---

### 3. Buyer Management

The system provides functionality for managing buyer/customer information.

Users can:

- Add new buyers
- View buyer details
- Search for buyers
- Update buyer information
- Delete buyer records
- Select existing buyers from stored database information

---

### 4. Product Management

The system provides functionality for managing product records.

Users can:

- Add new products
- View product details
- Search for products
- Update product information
- Delete products
- Work with product information stored in the database

---

### 5. Search and Database Suggestions

The system includes search and suggestion functionality to make it easier to find existing records.

Users can enter the **first letter or part of a buyer's name** to search for relevant records.

The application can also use information entered by the user to retrieve matching records from the database and suggest existing names.

This reduces the need to manually enter complete information and makes the application easier to use.

---

### 6. Tooltips

Helpful tooltip text has been added to different controls in the application.

When the user places the cursor over supported buttons or controls, a short description appears explaining the purpose of that control.

This improves usability and helps users understand the interface without needing separate instructions.

---

### 7. Billing System

The billing section allows the user to create a bill using buyer and product information.

The system uses information stored in the MySQL database while preparing the bill.

The billing process allows the user to:

- Select buyer information
- Select product information
- Enter billing details
- Work with stored product information
- Generate an invoice after completing the bill

---

### 8. Automatic PDF Invoice Generation

One of the main features of this project is automatic PDF invoice generation using **iTextPDF**.

After completing a bill, the system generates a PDF invoice containing the relevant billing information.

The generated PDF includes:

- Customer/buyer information
- Product information
- Billing information
- Actual date of invoice generation
- Actual time of invoice generation

The system also automatically names the generated PDF using the **customer's name followed by the actual date**.

For example:

```text
Amina_2026-07-27.pdf

---

## Technologies Used

| Technology | Purpose |
|---|---|
| Java | Core application development |
| MySQL | Database management |
| JDBC | Connecting Java with MySQL |
| iTextPDF | PDF invoice generation |

---
## Project Structure

semester-2-billing-management-system/
│
├── Database/
│   └── bms.sql
│
├── Demo/
│   └── BillingManagementSystem-Demo.mp4
│
├── Screenshots/
│   ├── Login.png
│   ├── Home.png
│   ├── BuyerDetails.png
│   ├── ProductDetails.png
│   ├── Billing.png
│   └── ...
│
├── nbproject/
│
├── src/
│   ├── Project/
│   │   └── ConnectionProvider.java
│   │
│   ├── billing/
│   │   └── Billing.java
│   │
│   ├── Login.java
│   ├── home.java
│   ├── newBuyer.java
│   ├── newProduct.java
│   ├── buyersDetails.java
│   ├── productDetails.java
│   ├── updateBuyer.java
│   ├── updateProduct.java
│   ├── deleteBuyer.java
│   ├── deleteProduct.java
│   ├── pdfWritter.java
│   └── GUI resources
│
├── test/
├── build.xml
├── manifest.mf
├── .gitignore
├── LICENSE
└── README.md

## Author

Amina Batool

Software Engineering Student
Riphah International University

GitHub:
https://github.com/Amina-SE