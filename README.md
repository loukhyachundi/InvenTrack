
# 📦 InvenTrack

**InvenTrack** is a robust Java-based Inventory Management System (IMS) designed for desktop environments using **Swing** and **JDBC**. It provides administrators and users with tools to manage employees, suppliers, categories, products, and sales — all within a user-friendly GUI.

---

## 🎯 Key Features

* Secure login with user role detection (Admin/User)  

* Real-time dashboards for employees, suppliers, sales, revenue, and more  

* Graphical user interface built with Java Swing  

* Profile-based login view with user image display  

* Dynamic full-screen resizing for enhanced usability  

* Role-based redirection to different dashboards  

* Modular design for managing Employees, Suppliers, Products, Categories, and Sales  

---

## 🧱 Tech Stack

### Backend

* **Java (JDK 8+)** – Core programming language  

* **JDBC (Java Database Connectivity)** – For connecting to the backend database  

* **MySQL / SQLite** – (expected) database for persistent storage  

* **Timer and TimerTask** – For real-time data updates  

### Frontend

* **Java Swing** – Desktop GUI development  

* **ImageIcon & Toolkit** – Image rendering and full-screen adaptation  

---

## 🔐 Authentication & User Roles

The system verifies login credentials by querying the `emp_ims` table and checks:

* `ID` (Username)  

* `Password`  

* `Usertype` – Either **Admin** or **User**  

Based on role, the user is redirected to:

* `Dashboard1` (Admin)  

* `Dashboard2` (User)  

Incorrect credentials trigger appropriate alerts for ID or password errors.

---

## 🖥️ Modules in Dashboard

The Admin Dashboard (`Dashboard1`) includes:

* Employee Management  

* Supplier Management  

* Category Management  

* Product Management  

* Sales Tracking  

* Logout  

Each module is a separate UI screen with backend logic, likely connected to relevant database tables.

---

## 🚀 Getting Started

### Requirements

* Java JDK 8 or higher  

* MySQL or SQLite (with required schema)  

* IDE (like NetBeans or IntelliJ IDEA)

### Run Locally

1. Clone the repository or import the source files into your IDE  
2. Ensure the database is set up and connection strings are updated  
3. Run the `Login` class or `Dashboard1` for admin testing  

---

## 📂 File Structure (Key Classes)

* `Login.java` – Handles login and user verification  

* `Dashboard1.java` – Admin dashboard with stats and module access  

* `DBConnection.java` – Utility class for database connection  

* `Employees.java`, `Suppliers.java`, etc. – Functional modules (expected)  

---

## 📸 UI Highlights

* Dynamic full-screen GUI  

* Graphical menus and buttons  

* Live employee and sales count updates  

* Profile photo loading using `ImageIcon`  

---

## 🙌 Acknowledgements

This project was developed as part of an academic or personal effort to create a complete inventory system using core Java and database skills.  
