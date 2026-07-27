# 🧾 Billing Management System

> A Java desktop-based Billing Management System developed as part of my **Object-Oriented Programming (OOP)** coursework during my 2nd semester at **Riphah International University**.

The project started as an OOP-based Java application and was later extended with **MySQL database integration, JDBC connectivity, search and suggestion functionality, interactive tooltips, animated navigation, and automated PDF invoice generation using iTextPDF**.

---

## 📌 Project Overview

The **Billing Management System** is a Java Swing desktop application designed to manage buyers, products, and billing operations through a graphical user interface.

The application provides a complete workflow for managing records and generating customer invoices.

### ✨ Main Highlights

- 🔐 Login system
- 🏠 Animated home-page navigation
- 👤 Buyer/customer management
- 📦 Product management
- 🔎 Search functionality
- 💡 Database-based suggestions
- 🖱️ Interactive tooltips
- 🧾 Billing and invoice generation
- 📄 Automatic PDF generation using iTextPDF
- 🕒 Automatic date and time recording
- 💾 Automatic PDF file naming
- 🗄️ MySQL database integration
- 🖥️ Java Swing graphical interface

> **Note:** The MySQL database integration and additional functionality were incorporated independently to extend the original OOP project and gain practical experience with database connectivity.

---

# 🚀 Features

## 🔐 1. Login System

The application starts with a login interface that provides access to the main system.

The login screen acts as the entry point to the application before the user can access the main features.

---

## 🏠 2. Animated Home Page Menu

The home page contains a menu of icons representing the different functions available in the system.

The navigation menu uses a simple sequential animation.

### How it works:

1. The user clicks the first icon.
2. The first menu item appears.
3. The remaining menu icons appear sequentially.
4. Each icon appears after an approximately **3–4 second delay**.
5. The complete menu is then available for navigation.

This creates a simple animated introduction to the application's main functions.

The menu provides access to features such as:

- 👤 Buyer Management
- 📦 Product Management
- 🧾 Billing
- 🔎 Buyer Details
- 🔎 Product Details
- ✏️ Update Operations
- 🗑️ Delete Operations
- 🚪 Logout

---

## 👤 3. Buyer Management

The Buyer Management section allows the user to manage customer/buyer records stored in the database.

### Available operations:

- ➕ Add new buyers
- 👁️ View buyer details
- 🔎 Search buyers
- ✏️ Update buyer information
- 🗑️ Delete buyer records
- 📋 Retrieve existing buyer information

---

## 📦 4. Product Management

The Product Management section allows the user to manage products stored in the MySQL database.

### Available operations:

- ➕ Add new products
- 👁️ View product details
- 🔎 Search products
- ✏️ Update product information
- 🗑️ Delete products
- 📋 Retrieve existing product information

---

## 🔎 5. Search & Database Suggestions

The application includes search functionality to make it easier to find existing buyers and products.

Instead of entering a complete name, the user can enter the **first letter or part of a name** to search for matching records.

The system retrieves matching information from the database and can provide suggestions based on the entered information.


```markdown
### Example workflow

**User enters:**

`A`

⬇️

**System checks the database**

⬇️

**Matching names are retrieved**

⬇️

**User selects the required record**
```

This makes the system faster and easier to use while reducing unnecessary manual data entry.

---

## 💡 6. Tooltips

The application includes helpful tooltip text on different controls and buttons.

When the user places the cursor over a supported control, a short description appears explaining its purpose.

This provides additional guidance and improves the overall usability of the interface.

---

## 🧾 7. Billing System

The Billing section brings together the buyer and product information required to prepare an invoice.

The system uses information stored in the MySQL database while preparing the bill.

The billing workflow allows the user to:

Select buyer/customer information
Select product information
Enter billing details
Work with stored database records
Prepare the final bill
Generate an invoice PDF

---

## 📄 8. Automatic PDF Invoice Generation

One of the main features of the project is automatic PDF invoice generation using iTextPDF.

After completing a bill, the application generates a PDF invoice containing the relevant billing information.

The generated invoice includes:
👤 Customer/buyer information
📦 Product information
🧾 Billing information
📅 Actual date of invoice generation
🕒 Actual time of invoice generation

The application also automatically generates the PDF filename using the customer's name followed by the actual date.

```text
Example:
CustomerName_2026-07-27.pdf
```

This makes generated invoices easier to identify, organize, and retrieve.

---

## 🗄️ Database

The application uses MySQL for storing and managing buyer and product information.

Database Name
bms
Main Tables
buyer
product

The complete SQL database file is included in the repository:

```text
Database/bms.sql
```

The SQL file can be imported into MySQL to recreate the database structure and data required by the application.

🔗 Java–MySQL Connection

The application connects Java with MySQL using JDBC.

The database connection is handled through:

```text
src/Project/ConnectionProvider.java
```
---

## 🛠️ Technologies Used
Technology	Purpose
☕ Java	Core application development
🧩 Object-Oriented Programming	Application structure and programming concepts
🖥️ Java Swing	Graphical User Interface
🧰 NetBeans IDE	Development environment
🗄️ MySQL	Database management
🔗 JDBC	Java–MySQL connectivity
📄 iTextPDF	Automated PDF invoice generation
🎨 Java Forms	GUI form development
🌱 Git & GitHub	Version control and project management

---

📁 Project Structure
```text
semester-2-billing-management-system/
│
├── 📂 Database/
│   └── bms.sql
│
├── 📂 Demo/
│   └── BillingManagementSystem-Demo.mp4
│
├── 📂 Screenshots/
│   ├── Login.png
│   ├── Home.png
│   ├── BuyerDetails.png
│   ├── ProductDetails.png
│   ├── Billing.png
│   └── ...
│
├── 📂 nbproject/
│
├── 📂 src/
│   │
│   ├── 📂 Project/
│   │   └── ConnectionProvider.java
│   │
│   ├── 📂 billing/
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
├── 📂 test/
│
├── build.xml
├── manifest.mf
├── .gitignore
├── LICENSE
└── README.md
```
---

# ⚙️ How to Run
## 📋 Requirements

Before running the application, make sure you have:

☕ Java JDK
🧰 NetBeans IDE
🗄️ MySQL Server
📄 iTextPDF library/dependencies
1️⃣ Clone the Repository
```text
git clone https://github.com/Amina-SE/semester-2-billing-management-system.git
```

2️⃣ Open the Project

Open the cloned project in NetBeans IDE.

The project follows the standard NetBeans Java project structure.

3️⃣ Set Up the Database

Create a MySQL database named:
```text
CREATE DATABASE bms;
```

Then import the SQL file:
```text
Database/bms.sql
```

This will recreate the required database tables and data.

4️⃣ Configure the Database Connection

Open:
```text
src/Project/ConnectionProvider.java
```

Update the MySQL username, password, and connection details according to your local MySQL configuration.


5️⃣ Run the Application

Build and run the project through NetBeans.

Once the application starts, use the login screen to access the main system.

---

## 🧠 OOP Concepts Practiced

This project was initially developed as part of my Object-Oriented Programming coursework.

The project provided practical experience with:

Classes and Objects
Encapsulation
Methods
Constructors
Object interaction
Modular program organization
Event-driven programming
GUI development
Exception handling
Database connectivity

The project also demonstrated how OOP concepts can be combined with GUI development, database connectivity, and external libraries to create a complete desktop application.

---

## 📚 What I Learned

This project helped me move from developing smaller Java programs toward building a more complete desktop application.

Key learning outcomes:
☕ Applying OOP concepts in a larger Java project
🖥️ Developing graphical interfaces using Java Swing
🧰 Working with NetBeans GUI forms
🗄️ Connecting Java applications to MySQL using JDBC
🔎 Searching and retrieving database records
💡 Creating database-based suggestions
🖱️ Improving usability through tooltips
📄 Working with external Java libraries
🧾 Generating PDF documents using iTextPDF
📅 Working with actual date and time values
📁 Automatically naming generated PDF files
🧩 Organizing a multi-screen desktop application
🌱 Using Git and GitHub for project management and version control

---

## 🔮 Future Improvements

Some possible future improvements include:

🔐 Improved authentication and password security
👥 Role-based access control
📦 Inventory and stock management
📊 Sales history and reporting
🔎 Advanced search and filtering
📈 Dashboard statistics
🎨 Improved invoice design
💾 Automated database backup and restore
✨ Improved UI/UX
🔒 Better database security
📑 More comprehensive reporting

---

## 👩‍💻 Author
Amina Batool

Software Engineering Student
Riphah International University


🔗 GitHub:
https://github.com/Amina-SE

📜 License

<div align="center">
This project is available under the license included in this repository.

⭐ Thanks for visiting this project!

If you found this project interesting, feel free to explore the repository and check out the demo and screenshots.

Built with Java ☕ • MySQL 🗄️ • JDBC 🔗 • iTextPDF 📄

</div> 