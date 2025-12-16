# Real Estate Manager (SQLite Edition) 🏠

A **C# Windows Forms** application designed to manage real estate property listings. This project demonstrates how to integrate a local **SQLite** database with a .NET application to perform **CRUD** (Create, Read, Update, Delete) operations securely and efficiently.

## 🚀 Features

### 1. Database Management 🗄️
* **Auto-Initialization:** Automatically generates the SQLite database file (`.db`) and the necessary tables if they do not exist.
* **Persistent Storage:** Data remains saved even after closing the application.

### 2. Dynamic User Interface 🎨
* **Programmatic UI Generation:** Labels and UI elements are generated and positioned **dynamically via code** (runtime) rather than being static in the designer.
* **User-Friendly Feedback:** Clear success/error messages via Message Boxes.

### 3. Data Operations (CRUD) 📝
* **Insert Property:** Allows users to input:
    * Price (€)
    * Address
    * Square Meters ($m^2$)
    * Description (Detailed text)
* **View Listings:** Retrieves data from the database and formats it into a readable list inside a `RichTextBox`.

## 🛡️ Technical Highlights

* **SQL Injection Protection:** Uses **Parameterized Queries** (e.g., `@price`, `@address`) to prevent security vulnerabilities.
* **Resource Management:** Utilizes `using` statements to ensure Database Connections are opened and closed automatically, preventing memory leaks.
* **Error Handling:** `Try-Catch` blocks are implemented to handle invalid user input (e.g., entering text instead of numbers).

## 📦 How to Run

1.  **Clone** the repository to your local machine.
2.  Open the solution file (`.sln`) in **Visual Studio**.
3.  **Restore NuGet Packages:**
    * Right-click on the Solution in the Solution Explorer.
    * Select **"Restore NuGet Packages"**.
    * *Note: This is required to download the `System.Data.SQLite` library automatically.*
4.  Press **Start** to run the application.

## 🖼️ Usage Guide

1.  Click **"1. Δημιουργία Βάσης"** to initialize the database.
2.  Fill in the text boxes (Price, Address, Sq. Meters, Description).
3.  Click **"2. Αποθήκευση"** to save the property.
4.  Click **"3. Εμφάνιση"** to see all saved properties in the list.

## 🛠️ Tech Stack
* **Language:** C#
* **Framework:** .NET Windows Forms
* **Database:** SQLite (`System.Data.SQLite`)

---
*University of Piraeus Project*
