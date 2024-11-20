# Nimap Machine Test - E-commerce CRUD API

This is a Spring Boot based RESTful API for managing **Categories** and **Products** in an e-commerce platform. The API supports CRUD operations, implements server-side pagination, and establishes a **one-to-many relationship** between categories and products. The project uses **Spring Boot**, **JPA**, and **Hibernate** for efficient backend operations and **MySQL** for the database.

## Features

- **Category CRUD Operations**: Create, read, update, and delete categories.
- **Product CRUD Operations**: Create, read, update, and delete products.
- **One-to-Many Relationship**: A category can have multiple products.
- **Server-side Pagination**: Pagination support for fetching categories and products.
- **Category and Product Linking**: Product details include their respective category data.

## Tech Stack

- **Backend**: Java, Spring Boot, Spring Data JPA, Hibernate
- **Database**: MySQL
- **Pagination**: Spring Data Pageable for server-side pagination
- **Tools**: IntelliJ IDEA, Postman for testing

## API Endpoints

### Category CRUD Operations

1. **Get All Categories (with Pagination)**  
   `GET http://localhost:8080/api/categories?page={pageNumber}`  
   Fetch all categories with server-side pagination. Example: `http://localhost:8080/api/categories?page=3`.

2. **Create a New Category**  
   `POST http://localhost:8080/api/categories`  
   Create a new category. Request body example:
   ```json
   {
     "name": "Electronics",
     "description": "All electronic products"
   }
