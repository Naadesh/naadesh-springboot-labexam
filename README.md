
Here’s a human-friendly and professional README file for your repository:

Spring Boot Lab Exam - Update Book Application
Project Overview
This project is a Spring Boot application developed as part of a lab exam. The application allows updating book details using a PUT request while following the MVC architecture. The backend uses JPA for database interactions and MySQL for persistent storage. The project has been tested using the Postman API tool.

Features
Implements CRUD functionality with a focus on update operation.
Built using MVC architecture:
Model: Defines the Book entity.
Controller: Handles HTTP requests.
Service: Contains business logic.
Repository: Manages database operations via JPA.
Uses MySQL as the database with configurations provided in application.properties.
Book Entity Properties
Book ID: Unique identifier for each book.
Title: Name of the book.
Author: Author of the book.
Genre: Category of the book.
Price: Cost of the book.
Published Year: Year the book was published.
Technology Stack
Java
Spring Boot
JPA (Java Persistence API)
MySQL Database
Postman (for API testing)
Setup Instructions
1. Clone the Repository
bash
Copy code
git clone https://github.com/naadesh/naadesh-springboot-labexam.git
cd naadesh-springboot-labexam
2. Configure the Database
Create a database named labexam in MySQL.
Update application.properties with your MySQL username and password:
properties
Copy code
spring.datasource.url=jdbc:mysql://localhost:3306/labexam
spring.datasource.username=yourusername
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
3. Insert Initial Data
Run the following SQL query to insert sample data into the book table:

sql
Copy code
INSERT INTO book (book_id, title, author, genre, price, published_year) 
VALUES (1, 'Spring Boot Basics', 'John Doe', 'Programming', 500, 2023);
4. Run the Application
bash
Copy code
mvn spring-boot:run
API Usage
Update a Book (PUT Request)
Endpoint: http://localhost:8080/api/books/{id}

Replace {id} with the ID of the book to update.
Request Body (JSON):

json
Copy code
{
  "title": "Advanced Spring Boot",
  "author": "Jane Doe",
  "genre": "Programming",
  "price": 650,
  "publishedYear": 2024
}
Response:
The updated book details will be returned in JSON format.

Testing
Use Postman to test the PUT endpoint.
Ensure the database is updated successfully after sending the request.
Repository Structure
bash
Copy code
src/
├── main/
│   ├── java/com/klef/jfsd/exam/
│   │   ├── model/        # Book entity
│   │   ├── repository/   # JPA repository
│   │   ├── service/      # Business logic
│   │   ├── controller/   # API endpoints
│   ├── resources/
│       ├── application.properties  # Database configuration
Author
Naadesh
