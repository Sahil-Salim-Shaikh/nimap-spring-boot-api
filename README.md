# Nimap Machine Test - E-commerce CRUD API

This is a Spring Boot-based RESTful API for managing **Categories** and **Products** in an e-commerce platform. The API supports CRUD operations, implements server-side pagination, and establishes a **one-to-many relationship** between categories and products. The project uses **Spring Boot**, **JPA**, and **Hibernate** for efficient backend operations and **MySQL** for the database.

## Features

- **Category CRUD Operations**: Create, read, update, and delete categories.
- **Product CRUD Operations**: Create, read, update, and delete products.
- **One-to-Many Relationship**: A category can have multiple products.
- **Server-side Pagination**: Pagination support for fetching categories and products.
- **Category and Product Linking**: Product details include their respective category data.
- **Exception Handling**: Graceful handling of errors with proper HTTP status codes and meaningful error messages.

## Tech Stack

- **Backend**: Java, Spring Boot, Spring Data JPA, Hibernate
- **Database**: MySQL
- **Pagination**: Spring Data Pageable for server-side pagination
- **Tools**: Eclipse IDE, Postman for testing

## API Endpoints

### Category CRUD Operations

1. **Get All Categories (with Pagination)**  
   `GET http://localhost:8080/api/categories?page={pageNumber}`  

2. **Create a New Category**  
   `POST http://localhost:8080/api/categories`  

3. **Get Category by ID**  
   `GET http://localhost:8080/api/categories/{id}`  

4. **Update Category by ID**  
   `PUT http://localhost:8080/api/categories/{id}`  

5. **Delete Category by ID**  
   `DELETE http://localhost:8080/api/categories/{id}`  

---

### Product CRUD Operations

1. **Get All Products (with Pagination)**  
   `GET http://localhost:8080/api/products?page={pageNumber}`  

2. **Create a New Product**  
   `POST http://localhost:8080/api/products`  

3. **Get Product by ID**  
   `GET http://localhost:8080/api/products/{id}`  

4. **Update Product by ID**  
   `PUT http://localhost:8080/api/products/{id}`  

5. **Delete Product by ID**  
   `DELETE http://localhost:8080/api/products/{id}`  

---
