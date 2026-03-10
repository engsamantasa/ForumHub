# 💬 FórumHub API

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/spring%20boot-%236DB33F.svg?style=for-the-badge&logo=springboot&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%234479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=Hibernate&logoColor=white)

## 📌 Overview
**FórumHub** is a robust RESTful API developed as a challenge for the **Oracle Next Education (ONE)** program in partnership with **Alura**. It replicates the back-end logic of a forum, allowing users to interact through topics categorized by courses.

This project demonstrates advanced knowledge in **Spring Boot 3**, focusing on clean architecture, stateless authentication with **JWT**, and complex business rules validation.

## ✨ Features
- **Stateless Authentication:** Secure login system using **Spring Security** and **JWT (JSON Web Tokens)**.
- **Advanced CRUD Management:** - Full management of discussion topics.
  - **Soft Delete (Logical Exclusion):** Topics are not physically removed from the database, preserving data integrity and audit trails.
  - **Pagination & Sorting:** Optimized endpoints returning paginated results (10 per page) sorted by creation date.
- **Security & Privacy:** - Sensitive data protection with **BCrypt** password hashing.
  - Prevention against duplicate topics (Title/Message validation).
- **Global Error Handling:** Customized response for common API errors (404 Not Found, 400 Bad Request, etc.).
- **Database Versioning:** Managed by **Flyway** for reliable schema migrations.

## 🚀 API Endpoints

### 🔐 Authentication
| Method | Endpoint | Description | Access |
| :--- | :--- | :--- | :--- |
| `POST` | `/login` | Authenticates user and returns a JWT Token | Public |

### 📝 Topics
| Method | Endpoint | Description | Access |
| :--- | :--- | :--- | :--- |
| `GET` | `/topicos` | Lists all active topics (Paginated & Sorted) | JWT |
| `GET` | `/topicos/{id}` | Detailed view of a specific topic | JWT |
| `POST` | `/topicos` | Creates a new discussion topic | JWT |
| `PUT` | `/topicos/{id}` | Updates topic title and message | JWT |
| `DELETE` | `/topicos/{id}` | Performs logical deletion (Deactivates topic) | JWT |

## 🛠️ Technologies & Tools
- **Java 17** (OpenJDK)
- **Spring Boot 3.x**
- **Spring Security** (Authentication & Authorization)
- **Spring Data JPA** (Persistence)
- **Auth0 Java JWT** (Token management)
- **MySQL** (Relational Database)
- **Flyway** (Database Migrations)
- **Lombok** (Boilerplate reduction)
- **Maven** (Dependency management)

## 🧑‍💻 Author
Developed by Samanta Sá 
**Computer Engineer & Full Stack Developer**
