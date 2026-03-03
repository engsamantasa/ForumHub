# 💬 FórumHub API

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/spring%20boot-%236DB33F.svg?style=for-the-badge&logo=springboot&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)

## 📌 Overview
FórumHub is a RESTful API built with **Spring Boot** that replicates the back-end functionality of a discussion forum. It provides a secure platform where registered users can create, read, update, and delete (CRUD) topics related to specific courses.

This project focuses heavily on **Data Persistence**, **Business Rules Validation**, and **Security**, ensuring that only authenticated users can manage topics, and strictly limiting modification/deletion rights to the original authors.

## ✨ Features
- **User Authentication & Authorization:** Secure login system generating stateless JWT (JSON Web Tokens).
- **Topic Management (CRUD):** - Create new discussion topics.
  - Retrieve all topics or search for specific ones.
  - Update topic details (restricted to the author).
  - Delete topics (restricted to the author).
- **Data Integrity:** Relational database mapping using Spring Data JPA.
- **Input Validation:** Strict validation of incoming JSON payloads to ensure data consistency.


## 🛠️ Technologies & Tools
- **Java 17**
- **Spring Boot 3** (Web, Data JPA, Security, Validation)
- **Spring Security & JWT (Auth0)** for Authentication
- **Flyway** for Database Migrations
- **MySQL** as the Relational Database
- **Lombok** to reduce boilerplate code


## 🧑‍💻 Author
Developed by Samanta Sá

