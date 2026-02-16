# 🛒 Product Service - DevOps Lab 03

## 📌 Project Overview

This project is a Spring Boot microservice developed for DevOps Lab 03 at SLIIT.

It implements a RESTful API to manage products using CRUD operations.

The application includes:
- Spring Boot REST API
- H2 In-Memory Database
- Swagger (Springdoc OpenAPI) for API documentation
- Full CRUD functionality (Create, Read, Delete)

---

## 🛠️ Technologies Used

- Java 17
- Spring Boot 4.0.2
- Spring Web
- Spring Data JPA
- H2 In-Memory Database
- Swagger (Springdoc OpenAPI)
- Maven
- Git & GitHub

---

## 🚀 Features Implemented

✔ Create Product (POST)  
✔ Get All Products (GET)  
✔ Get Product by ID (GET)  
✔ Delete Product (DELETE)  
✔ Swagger UI for API Testing  
✔ H2 Console for Database Verification  

---

## 📂 Project Structure

```
product-service
│
├── .mvn
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── sliit
│   │   │           └── product_service
│   │   │               ├── controller
│   │   │               │   └── ProductController.java
│   │   │               ├── entity
│   │   │               │   └── Product.java
│   │   │               ├── repository
│   │   │               │   └── ProductRepository.java
│   │   │               └── ProductServiceApplication.java
│   │   └── resources
│   │       └── application.properties
│   │
│   └── test
│       └── java
│           └── com
│               └── sliit
│                   └── product_service
│                       └── ProductServiceApplicationTests.java
│
├── pom.xml
├── mvnw
├── mvnw.cmd
├── .gitignore
└── README.md
```

---

## ⚙️ How to Run the Application

### 1️⃣ Clone the Repository

```
git clone https://github.com/username/product-service.git
```

### 2️⃣ Navigate to Project Folder

```
cd product-service
```

### 3️⃣ Run the Application

```
mvn spring-boot:run
```

The application will start at:

```
http://localhost:8080
```

---

## 📖 Swagger API Documentation

After running the application, open:

```
http://localhost:8080/swagger-ui/index.html
```

You can test all REST endpoints directly using Swagger UI.

---

## 🗄️ H2 Database Console

Open:

```
http://localhost:8080/h2-console
```

Use the following credentials:

- JDBC URL: `jdbc:h2:mem:productdb`
- Username: `sa`
- Password: `########`

Example SQL Query:

```sql
SELECT * FROM PRODUCTS;
```

---

## 🔗 Available API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST   | /api/products | Create new product |
| GET    | /api/products | Get all products |
| GET    | /api/products/{id} | Get product by ID |
| DELETE | /api/products/{id} | Delete product by ID |

---

## 📝 Example JSON Request Body

```json
{
  "name": "Mouse",
  "price": 2500
}
```

---

## 🎯 Lab Objectives Achieved

✔ Spring Boot project creation using Spring Initializr  
✔ RESTful API implementation  
✔ H2 in-memory database integration  
✔ Swagger integration  
✔ CRUD operations successfully tested  

---

## 👩‍💻 Author

AMBEGODA A.L.A.S.K
