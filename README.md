# EcoReport – Public Infrastructure & Fire Incident Reporting System

## 📍 Overview

EcoReport is a full-stack web application designed to improve communication between citizens and local authorities in the Province of Ifrane.

The platform allows citizens to report public infrastructure issues such as water leaks, fire hazards, and damaged public property, while enabling administrators to manage, prioritize, and resolve these reports efficiently.

---

## 🎯 Problem

In Ifrane, there is no centralized system for citizens to report infrastructure problems.
As a result:

* Water leaks go unnoticed for long periods
* Fire hazards are not reported quickly
* Public infrastructure issues remain unresolved

---

## 💡 Solution

EcoReport provides:

* A structured platform for submitting incident reports
* Real-time tracking of report status
* An admin dashboard for managing reports
* A points and certification system to encourage citizen participation

---

## ⚙️ Features

### 👤 Citizen

* Register and login (JWT authentication)
* Submit reports with:

  * Incident type (water, fire, infrastructure)
  * Description
  * Location (map-based)
  * Photo upload
* Track report status (Pending / In Progress / Resolved)
* Earn points for valid reports
* Receive certificates (Bronze / Silver / Gold)

### 🛠️ Admin

* View all reports in a centralized dashboard
* Filter by type, status, and priority
* Update report status and priority
* Validate reports and award points

---

## 🏗️ Architecture

The system follows a **4-layer architecture**:

1. **Presentation Layer**

   * HTML, CSS, JavaScript
   * User and admin interfaces

2. **Controller Layer**

   * REST APIs using Spring Boot

3. **Service Layer**

   * Business logic (validation, points system, location checks)

4. **Data Access Layer**

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

* `users`
* `reports`
* `certificates`
* `points_transactions`

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

* Navigate to the backend folder
* Run the Spring Boot application:

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
* Import the SQL schema provided
* Update database credentials in `application.properties`

---

### 3. Frontend

* Open the frontend folder
* Run using Live Server (or open `index.html`)

Frontend runs on:

```
http://localhost:5500
```

---

## 📌 Current Status

The system is fully implemented:

* Backend and frontend are functional
* Database is connected and populated

🔧 **Known Issue:**
Authentication login fails due to a BCrypt hash mismatch in the database.
This is a data issue and can be resolved by updating the stored password hash.

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

* Fix authentication issue
* Deploy application online
* Add real-time notifications
* Improve UI/UX design
* Mobile version

---

## 🔗 Repository Link

(Add your GitHub link here)
