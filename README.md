# **Spring Boot Lab Exam - Update Book Application**

## **Project Overview**  
This project is a Spring Boot application developed as part of a lab exam. The application allows updating book details using a **PUT request** while following the **MVC architecture**. The backend uses JPA for database interactions and MySQL for persistent storage. The project has been tested using the Postman API tool.

---

## **Features**  
- Implements CRUD functionality with a focus on **update operation**.  
- Built using **MVC architecture**:
  - **Model:** Defines the `Book` entity.
  - **Controller:** Handles HTTP requests.
  - **Service:** Contains business logic.
  - **Repository:** Manages database operations via JPA.
- Uses **MySQL** as the database with configurations provided in `application.properties`.

---

## **Book Entity Properties**  
- **Book ID**: Unique identifier for each book.
- **Title**: Name of the book.
- **Author**: Author of the book.
- **Genre**: Category of the book.
- **Price**: Cost of the book.
- **Published Year**: Year the book was published.

---

## **Technology Stack**  
- **Java**  
- **Spring Boot**  
- **JPA (Java Persistence API)**  
- **MySQL Database**  
- **Postman (for API testing)**  

---

## **Setup Instructions**  

### 1. Clone the Repository  
```bash
git clone https://github.com/naadesh/naadesh-springboot-labexam.git
cd naadesh-springboot-labexam
