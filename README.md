
# Employee Management System - Spring Boot & Thymeleaf 🧑‍💼👨‍💻

A simple Employee Management System built using **Spring Boot** and **Thymeleaf** for managing employee data via a web interface. This project demonstrates basic CRUD operations (Create, Read, Update, Delete) with a clean and dynamic UI using Thymeleaf templates.

## 🚀 Live Demo

![Live Demo Screenshot](https://github.com/babureddynr/employee-management-system-springboot-Thymleaf/blob/main/demo_screenshot.png)

> _Screenshot of the live running demo of Employee Management System_.

---

## 📑 Project Description

The **Employee Management System** allows you to manage employee information with features like adding new employees, viewing existing ones, updating employee details, and deleting them. The system is built using **Spring Boot** for the backend API, and **Thymeleaf** for rendering dynamic HTML pages. Data is stored in an **H2 in-memory database** (can be configured for MySQL).

### 🔧 Features:
- 📝 **Create** new employees.
- 📄 **Read** employee details in a list view.
- ✏️ **Update** employee information.
- 🗑️ **Delete** employees from the system.
- 🖼️ Dynamic web pages using **Thymeleaf**.
- 📊 **Spring Data JPA** integration for database interactions.
- ⚡ **RESTful API** for employee management.

---

## 🛠️ Tech Stack

- **Spring Boot** - Backend logic and RESTful services.
- **Thymeleaf** - Frontend templating engine for dynamic web content.
- **Spring Data JPA** - ORM for database management.
- **H2** / **MySQL** - Database (in-memory or persistent).

---

## 📜 Endpoints

Here are the available API endpoints to manage employees via Postman or other REST clients:

### 📄 Fetch All Employees
**Endpoint:** `GET /employees`  
**Description:** Retrieves a list of all employees.  
**Usage Example:**  
```
GET http://localhost:8080/employees
```

### ➕ Add New Employee
**Endpoint:** `POST /employees/save`  
**Description:** Adds a new employee or updates an existing one.  
**Body Example (JSON):**
```json
{
    "name": "John Doe",
    "department": "HR"
}
```
**Usage Example:**  
```
POST http://localhost:8080/employees/save
```

### 🗑️ Delete Employee
**Endpoint:** `GET /employees/delete/{id}`  
**Description:** Deletes an employee by their ID.  
**Usage Example:**  
```
GET http://localhost:8080/employees/delete/1
```

---

## 📝 Setup & Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/babureddynr/employee-management-system-springboot-Thymleaf.git
   cd employee-management-system-springboot-Thymleaf
   ```

2. Build and run the project:
   ```bash
   ./mvnw spring-boot:run
   ```

3. Access the application in your browser:
   ```
   http://localhost:8080/employees
   ```

---

## 🔍 Testing with Postman

You can test the CRUD operations using Postman:

- **GET All Employees:**  
  ```
  GET http://localhost:8080/employees
  ```

- **POST Add Employee:**  
  ```json
  POST http://localhost:8080/employees/save
  Body (raw, JSON):
  {
      "name": "Jane Doe",
      "department": "Engineering"
  }
  ```

- **DELETE Employee by ID:**  
  ```
  GET http://localhost:8080/employees/delete/1
  ```

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

### 👨‍💻 Author

**Babu Reddy NR**
