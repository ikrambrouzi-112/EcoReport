# 🌍 EcoReport – Public Infrastructure & Fire Incident Reporting System

## 📍 Overview

**EcoReport** is a full-stack web application designed to improve communication between citizens and local authorities in the Province of Ifrane.

The platform enables citizens to report public infrastructure issues such as water leaks, fire hazards, and damaged public property, while allowing administrators to efficiently manage, prioritize, and resolve these reports.

---

## 🎯 Problem

In Ifrane, there is no centralized system for reporting infrastructure issues. As a result:

* Water leaks go unnoticed for long periods
* Fire hazards are not reported quickly
* Public infrastructure issues remain unresolved

---

## 💡 Solution

EcoReport provides:

* A structured platform for submitting incident reports
* Real-time tracking of report status
* An admin dashboard for efficient management
* A points and certification system to encourage citizen participation

---

## ⚙️ Features

### 👤 Citizen

* Register and login (JWT authentication)
* Submit reports with:

  * Incident type (water, fire, infrastructure)
  * Description
  * Location (map-based using Leaflet.js)
  * Photo upload
* Track report status (Pending / In Progress / Resolved)
* Earn points for valid reports
* Receive certificates (Bronze / Silver / Gold)

---

### 🛠️ Admin

* View all reports in a centralized dashboard
* Filter by type, status, and priority
* Update report status and priority
* Validate reports and award points

---
## 📸 Screenshots

### 🏠 Home Page

<img src="screenshots/Home.jpeg" width="700">

---

### 🔐 Login

<img src="screenshots/login.jpeg" width="700">

---

### 📊 User Dashboard

<img src="screenshots/dashboard.jpeg" width="700">

---

### 📝 Report Submission (Step 1)

<img src="screenshots/Report_Submission.jpeg" width="700">

---

### 📝 Report Submission (Step 2)

<img src="screenshots/Report_Submission2.jpeg" width="700">

---

### ✅ Submission Confirmation

<img src="screenshots/Submission.jpeg" width="700">

---

### 🛠️ Admin Dashboard

<img src="screenshots/Admin_Dashboard.jpeg" width="700">

---

### ⚙️ Admin Features

<img src="screenshots/Admin_features.jpeg" width="700">

---

### 📈 Report Management

<img src="screenshots/Report_Management.jpeg" width="700">

---

## 🏗️ Architecture

The system follows a **4-layer architecture**:

* **Presentation Layer**

  * HTML, CSS, JavaScript
  * User and admin interfaces

* **Controller Layer**

  * REST APIs using Spring Boot

* **Service Layer**

  * Business logic (validation, points system, location checks)

* **Data Access Layer**

  * MySQL database using JPA repositories

---

## 🧰 Technologies Used

### Backend

* Java 17
* Spring Boot
* Spring Security (JWT Authentication)
* Hibernate / JPA
* BCrypt (password hashing)

### Frontend

* HTML
* CSS
* JavaScript
* Leaflet.js (map integration)

### Database

* MySQL

---

## 🗄️ Database Design

Main tables:

* users
* reports
* certificates
* points_transactions

Includes:

* Foreign key constraints
* ENUM types for status and priority
* Data validation rules

---

## 🔐 Security

* JWT-based authentication
* Password hashing using BCrypt
* Role-based access control (Citizen / Admin)

---

## 🚀 How to Run the Project

### 1. Backend

Navigate to the backend folder and run:

```bash
mvn spring-boot:run
```

Server runs on:

```
http://localhost:8080
```

---

### 2. Database

* Create a MySQL database
* Import the provided SQL schema
* Update credentials in `application.properties`

---

### 3. Frontend

* Open the frontend folder
* Run using Live Server or open `index.html`

Frontend runs on:

```
http://localhost:5500
```

---

## 📌 Current Status

✅ Backend and frontend fully functional
✅ Database connected and populated
✅ Authentication issue fixed (BCrypt hashing corrected)

---

## 👥 Team Members

* Lalla Ibtihal Jerboui
* Ikram El Brouzi
* Oumaima Dehmane

---

## 🎓 Academic Context

Software Engineering Project
Al Akhawayn University – April 2026

---

## 📬 Future Improvements

* Deploy application online
* Add real-time notifications
* Improve UI/UX design
* Develop a mobile version

---
