# ✅ To-Do List Application (Spring Boot + Thymeleaf + MySQL)

A simple **To-Do List Web Application** built using **Spring Boot, Thymeleaf, and MySQL**.  
It supports **CRUD operations** (Create, Read, Update/Toggle, Delete) for managing daily tasks.  

---

## 🚀 Features
- Add new tasks
- Mark tasks as completed/incomplete
- Delete tasks
- Responsive UI with Bootstrap
- Data persistence with MySQL

---

## 🛠️ Tech Stack & Dependencies
- **Java 17/21/23** (Project language)
- **Spring Boot** (Framework)
- **Spring Web** → Build web applications and REST APIs
- **Spring Data JPA** → ORM for database operations
- **MySQL Driver** → Database connectivity
- **Lombok** → Reduces boilerplate code (getters/setters)
- **Thymeleaf** → Template engine for dynamic HTML
- **Maven** → Build and dependency management tool

---

## 📂 Project Structure
TodoApp/
│── src/main/java/com/example/Todo
│ ├── controller/
│ │ └── TaskController.java # Handles HTTP requests
│ ├── models/
│ │ └── Task.java # Task entity (DB table)
│ ├── repository/
│ │ └── TaskRepository.java # JPA Repository for DB operations
│ ├── services/
│ │ └── TaskService.java # Business logic
│ └── TodoApplication.java # Main application entry point
│
│── src/main/resources/
│ ├── templates/
│ │ └── tasks.html # Thymeleaf template (UI)
│ ├── static/ # (Optional) CSS/JS files
│ └── application.properties # DB configuration
│
│── pom.xml # Maven dependencies
│── README.md # Documentation

---

## ⚙️ Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/your-username/todo-springboot.git
cd todo-springboot
2. Configure MySQL Database
Create a database in MySQL:
CREATE DATABASE todoapp;
Update src/main/resources/application.properties:
spring.datasource.url=jdbc:mysql://localhost:3306/todoapp
spring.datasource.username=your-username
spring.datasource.password=your-password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
3. Build & Run
mvn clean install
mvn spring-boot:run
4. Access the App
Open your browser and visit:
👉 http://localhost:8080
