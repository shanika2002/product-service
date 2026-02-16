# Product Service - DevOps Lab 03

## 📌 Project Overview

This project is a Spring Boot microservice developed for DevOps Lab 03.  
It implements a RESTful API for managing products using CRUD operations.

The application uses:
- Spring Boot 4
- Spring Data JPA
- H2 In-Memory Database
- Swagger (Springdoc OpenAPI)

---

## 🚀 Features

- Create a Product (POST)
- Get All Products (GET)
- Get Product by ID (GET)
- Delete Product by ID (DELETE)
- Swagger UI for API testing
- H2 Console for database verification

---

## 🛠️ Technologies Used

- Java 17
- Spring Boot
- Spring Web
- Spring Data JPA
- H2 Database
- Maven
- Swagger (Springdoc OpenAPI)

---

## 📂 Project Structure

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

---

## ⚙️ How to Run the Application

1. Clone the repository:

git clone https://github.com/username/product-service.git


2. Navigate to the project folder:

cd product-service


3. Run the application:

mvn spring-boot:run


The application will start at:

http://localhost:8080

---

## 📖 API Documentation (Swagger UI)

Access Swagger UI at:

http://localhost:8080/swagger-ui/index.html

---

## 🗄️ H2 Database Console

Access H2 Console at:

http://localhost:8080/h2-console

Use the following credentials:

- JDBC URL: `jdbc:h2:mem:productdb`
- Username: `sa`
- Password: `########`

Example SQL query:

SELECT * FROM PRODUCTS;

---

## 🔗 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST   | /api/products | Create new product |
| GET    | /api/products | Get all products |
| GET    | /api/products/{id} | Get product by ID |
| DELETE | /api/products/{id} | Delete product by ID |

---

## 📝 Example JSON Request

{
  "name": "Mouse",
  "price": 2500
}


