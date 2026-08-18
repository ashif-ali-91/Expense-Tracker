# 💰 Expense Tracker — Spring Boot

A simple **Expense Tracker Backend** built using Java and Spring Boot.
This project is designed as a beginner-friendly backend project to learn REST APIs, Spring Data JPA, and MySQL.

## 🚀 Features

* Add a new expense
* View all expenses
* View expense by ID
* Update an expense
* Delete an expense
* Store expense data in MySQL
* RESTful API endpoints

## 🛠️ Technologies Used

* **Java 17**
* **Spring Boot**
* **Spring Web**
* **Spring Data JPA**
* **MySQL**
* **Maven**
* **Git & GitHub**
* **Postman**

## 📂 Project Structure

```text
expense-tracker
│
├── src
│   └── main
│       ├── java
│       │   └── com.example.expensetracker
│       │       ├── controller
│       │       │   └── ExpenseController.java
│       │       ├── model
│       │       │   └── Expense.java
│       │       ├── repository
│       │       │   └── ExpenseRepository.java
│       │       └── ExpenseTrackerApplication.java
│       │
│       └── resources
│           └── application.properties
│
├── pom.xml
└── README.md
```

## 🔗 API Endpoints

| Method | Endpoint         | Description       |
| ------ | ---------------- | ----------------- |
| POST   | `/expenses`      | Add a new expense |
| GET    | `/expenses`      | Get all expenses  |
| GET    | `/expenses/{id}` | Get expense by ID |
| PUT    | `/expenses/{id}` | Update an expense |
| DELETE | `/expenses/{id}` | Delete an expense |

## 📝 Example Request

### Add Expense

**POST**

```text
/expenses
```

Request body:

```json
{
  "title": "Lunch",
  "amount": 250,
  "category": "Food",
  "date": "2026-08-18"
}
```

Example response:

```json
{
  "id": 1,
  "title": "Lunch",
  "amount": 250,
  "category": "Food",
  "date": "2026-08-18"
}
```

## 🗄️ Database Setup

Create a MySQL database:

```sql
CREATE DATABASE expense_db;
```

Update your `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/expense_db
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

Replace `YOUR_PASSWORD` with your local MySQL password.

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/expense-tracker-spring-boot.git
```

### 2. Open the project

Open the project in **VS Code** or **IntelliJ IDEA**.

### 3. Configure MySQL

Create the `expense_db` database and update your database credentials in:

```text
src/main/resources/application.properties
```

### 4. Run the application

Using Maven:

```bash
mvn spring-boot:run
```

The application will run on:

```text
http://localhost:8080
```

## 🧪 Testing

The API can be tested using **Postman**.

Example:

```text
GET http://localhost:8080/expenses
```

## 🎯 Learning Objectives

This project helped me understand:

* Java backend development
* Spring Boot fundamentals
* REST API development
* HTTP methods
* Spring Data JPA
* CRUD operations
* MySQL database integration
* Maven
* Git and GitHub
* API testing with Postman

## 🔮 Future Improvements

Planned improvements:

* [ ] Service layer
* [ ] Input validation
* [ ] Global exception handling
* [ ] Search expenses by category
* [ ] Monthly expense summary
* [ ] User registration and login
* [ ] Spring Security
* [ ] JWT authentication
* [ ] Frontend interface
* [ ] Cloud deployment

## 👨‍💻 Author

**Ashif Ali**

Aspiring Java Backend Developer

---

⭐ If you find this project useful, feel free to give it a star!
