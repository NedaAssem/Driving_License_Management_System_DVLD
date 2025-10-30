# 🚗 Driving License Management System (DVLD)

## 📘 Overview
The **Driving License Management System (DVLD)** is a C# Windows Forms application that manages all operations related to driving licenses, such as issuing, renewing, replacing, and managing users and drivers.  
It follows a **3-tier architecture** and uses **ADO.NET** to interact with a **SQL Server LocalDB** database (`DVLD.mdf`).

---

## 🚗 Features

- **User Management:** Add, update, delete, or freeze user accounts with role-based permissions.  
- **Person Management:** Register new people and manage their personal information.  
- **License Services:**  
  - Issue new driving licenses for various categories.  
  - Renew, replace lost or damaged licenses.  
  - Release detained licenses.  
  - Issue international driving licenses.  
- **Application Management:** Create and track service requests with unique application numbers and fees.  
- **Testing & Scheduling:**  
  - Schedule vision, written, and practical driving tests.  
  - Record test results (pass/fail and score).  
  - Allow retesting for failed applicants after payment.  
- **Data Validation:** Ensure that each person has a unique national ID and no duplicate active license applications.  
- **Payment Management:** Handle and track service fees and test payments.  
- **Local Database (SQL Server):** Store all data locally using ADO.NET.  
- **Three-Tier Architecture:** Separation between UI, Business Logic, and Data Access layers for better organization and maintainability.

---

## 🧱 Technologies Used
- **C# (.NET Framework 4.7.2)**  
- **Windows Forms**  
- **ADO.NET** (SQL Connection, Command, Adapter, DataTable)  
- **SQL Server LocalDB**  

---

## 🧩 Project Structure
The project follows a **three-tier architecture** to improve organization and maintainability:
Project  
│  
├── DVLD → User Interface Layer (Windows Forms)   
│ ├── Applications  
│ ├── Drivers   
│ ├── Licenses   
│ ├── Login   
│ ├── People   
│ ├── Tests   
│ └── User   
│    
├── DVLD_Business → Business Logic Layer   
│ └── (Contains classes for managing system operations)  
│   
└── DVLD_DataAccess → Data Access Layer  
└── (Handles database connections using ADO.NET)   



---

## 🗄️ Database Setup
The system uses a local SQL Server database named `DVLD.mdf`.

### Steps to attach the database
1. Open **SQL Server Management Studio (SSMS)**.  
2. Right-click **Databases → Attach**.  
3. Browse to the project folder and select `DVLD.mdf`.  
4. Click **OK** to attach the database.  
5. Make sure your project connection string points to the correct database file.

Example connection string:

Data Source=(LocalDB)\MSSQLLocalDB;AttachDbFilename=|DataDirectory|\DVLD.mdf;Integrated Security=True;

---
##▶️ How to Run

1. Open the solution file DVLD.sln in Visual Studio.

2. Make sure the startup project is set to DVLD (the UI layer).

3. Check that the database DVLD.mdf is attached and the connection string is correct.

4. Press F5 or click Start to run the application.

5. Login using the credentials stored in the Users.txt file.

---

## 🔑 Login Information

The system requires a username and password to access the dashboard.  
Login data is stored in the file:

DVLD\bin\Debug


The file contains usernames and passwords in plain text.

Example credentials to test the system:

- **Username:** Msaqer77  
- **Password:** 1234

---

🖼️ Screenshots

You can include screenshots to demonstrate how the system works:

---

