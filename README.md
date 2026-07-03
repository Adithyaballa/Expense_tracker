# Expense_tracker
The Expense Tracker Application is a comprehensive solution designed to help users manage their finances efficiently by tracking expenses across different categories.

# 💰 Expense Tracker Application

A backend RESTful web application developed using **Java** and **Spring Boot** that helps users efficiently manage their daily expenses by organizing them into categories. The application provides secure and scalable REST APIs for performing CRUD operations on expenses and categories while implementing proper exception handling and API documentation.

---

## 🚀 Features

- 📂 Category Management (Create, Read, Update, Delete)
- 💵 Expense Management (Create, Read, Update, Delete)
- 🔍 Retrieve Expenses by ID and List All Expenses
- 📑 RESTful API Development using Spring Boot
- ⚠️ Global Exception Handling with Custom Error Responses
- 📖 Interactive API Documentation using Swagger (OpenAPI)
- 🗄️ Database Integration with MySQL using Spring Data JPA
- 🏗️ Layered Architecture (Controller → Service → Repository)

---

## 🛠️ Tech Stack

### Backend
- Java 21
- Spring Boot 3
- Spring Data JPA
- Hibernate ORM
- REST API
- Maven

### Database
- MySQL

### API Testing
- Postman
- Swagger UI (SpringDoc OpenAPI)

### Development Tools
- IntelliJ IDEA
- Git & GitHub

---

## 📂 Project Structure

```
Expense-Tracker
│
├── controller
├── service
├── repository
├── entity
├── dto
├── mapper
├── exception
├── config
└── resources
```

---

## 📌 Project Architecture

```
Client (Postman / Swagger)

        │
        ▼

 Controller

        │
        ▼

   Service Layer

        │
        ▼

 Repository (JPA)

        │
        ▼

     MySQL Database
```

---

## 📋 Modules

### 1️⃣ Category Management

- Create Category
- Update Category
- Delete Category
- Get Category by ID
- Get All Categories

### 2️⃣ Expense Management

- Add Expense
- Update Expense
- Delete Expense
- Get Expense by ID
- Get All Expenses

---

## 🔗 REST API Endpoints

### Category APIs

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/categories | Create Category |
| GET | /api/categories | Get All Categories |
| GET | /api/categories/{id} | Get Category by ID |
| PUT | /api/categories/{id} | Update Category |
| DELETE | /api/categories/{id} | Delete Category |

---

### Expense APIs

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/expenses | Create Expense |
| GET | /api/expenses | Get All Expenses |
| GET | /api/expenses/{id} | Get Expense by ID |
| PUT | /api/expenses/{id} | Update Expense |
| DELETE | /api/expenses/{id} | Delete Expense |

---

## ⚙️ Key Features

- RESTful API Development
- CRUD Operations
- DTO Pattern
- Entity Mapping
- Layered Architecture
- Dependency Injection
- Spring Data JPA
- Hibernate ORM
- Custom Exception Handling
- Global Exception Handler
- Swagger Documentation
- MySQL Integration

---

## ⚠️ Exception Handling

The application implements centralized exception handling using:

- @ControllerAdvice
- @ExceptionHandler
- Custom ResourceNotFoundException
- Standard HTTP Status Codes
- Structured JSON Error Responses

Example:

```json
{
  "timestamp": "2026-07-01T10:30:45",
  "message": "Expense not found with id: 5",
  "path": "/api/expenses/5",
  "errorCode": "RESOURCE_NOT_FOUND"
}
```

---

## 📖 API Documentation

Swagger UI is integrated for interactive API testing.

```
http://localhost:8080/swagger-ui/index.html
```

---

## 💾 Database

Database: MySQL

Example Tables:

- Categories
- Expenses

Spring Data JPA automatically manages database operations using Hibernate ORM.

---

## ▶️ How to Run the Project

### Clone Repository

```bash
git clone https://github.com/your-username/expense-tracker.git
```

### Navigate

```bash
cd expense-tracker
```

### Configure Database

Update:

```
application.properties
```

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/expense_tracker

spring.datasource.username=root

spring.datasource.password=your_password
```

### Build Project

```bash
mvn clean install
```

### Run

```bash
mvn spring-boot:run
```

Application starts at

```
http://localhost:8080
```

---

## 🧪 Testing

REST APIs were tested using:

- Postman
- Swagger UI

---

## 📈 Future Enhancements

- User Authentication (JWT)
- Spring Security
- Role-Based Access Control
- Monthly Expense Reports
- Expense Analytics Dashboard
- Budget Planning
- Email Notifications
- Docker Deployment
- CI/CD Pipeline
- Frontend using React.js

---

## 📚 Learning Outcomes

Through this project, I gained hands-on experience with:

- Java
- Spring Boot
- REST API Development
- Spring Data JPA
- Hibernate
- MySQL
- Exception Handling
- Swagger
- Maven
- Git & GitHub
- Layered Architecture
- DTO Pattern

---

## 👨‍💻 Author

**Balla Adithya**

Java Backend Developer

---

⭐ If you found this project useful, don't forget to Star this repository.
