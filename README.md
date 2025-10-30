# 🚘 Driving License Management System (DVLD)

## 📋 Overview
The Driving License Management System (DVLD) is a three-tier C# Windows Forms application that helps manage all operations related to driving licenses.  
It allows users to handle applications, manage tests, issue and renew licenses, and maintain records for drivers and staff.  
The system was built for academic learning purposes and focuses on database management, ADO.NET, and multi-layered application design.

---

## 🧩 Features

- **User Management:** Add, update, delete, or freeze user accounts with role-based permissions.  
- **Person Management:** Register new people and manage their personal information.  
- **License Services:**  
  - Issue new driving licenses for different categories.  
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

## 🏗️ Project Structure

Project  
│  
├───DVLD # User Interface (Windows Forms)  
│ ├───Applications  
│ ├───Drivers  
│ ├───Licenses  
│ ├───People  
│ ├───Login  
│ ├───Tests  
│ ├───User  
│ └───Global Classes  
│  
├───DVLD_Business # Business Logic Layer  
│  
└───DVLD_DataAccess # Data Access Layer (ADO.NET + SQL)  


---

## 🗃️ Database

- **Database Name:** `DVLD.mdf`  
- **Type:** SQL Server (LocalDB)  
- **Connection:** Uses ADO.NET with standard SQL queries and stored procedures.  
- The database contains tables for:
  - Persons  
  - Users  
  - Applications  
  - Licenses  
  - Tests  
  - Application Types  
  - License Classes  

> ⚠️ Make sure the `.mdf` file is properly attached to your SQL Server LocalDB instance before running the project.

---

## 🔐 Login Information

The login data is stored in the local text file: 

 DVLD\bin\Debug\data.txt

> Open this file to find the default usernames and passwords used for logging into the system.

Example credentials:

- **Username:** Msaqer77  
- **Password:** 1234
---

## ⚙️ Technologies Used

- **Language:** C#  
- **Framework:** .NET Framework 4.7.2  
- **Database:** SQL Server LocalDB (`.mdf`)  
- **Data Access:** ADO.NET  
- **Architecture:** 3-Tier (Presentation, Business Logic, Data Access)  
- **IDE:** Visual Studio  

---

## 🧠 Purpose

This project was developed for learning purposes to understand:
- How to design a real-world system with layered architecture.  
- How to use ADO.NET for data management.  
- How to organize a medium-size C# project.  

---

## 📸 Screenshots (Optional)

You can add screenshots of your system here by uploading images to your repository and using this format:

```markdown
![Login Screen](images/login_screen.png)
![Main Dashboard](images/dashboard.png)

## 🧾 License

This project is created for educational use and is not intended for commercial distribution.

  
