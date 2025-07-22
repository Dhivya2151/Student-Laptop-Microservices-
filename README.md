# Student-Laptop-Microservices:-
This is a Spring Boot microservice that manages **Students** and their associated **Laptops**. It provides REST APIs for CRUD operations and integrates with other services using **OpenFeign** and **Eureka Server**.

## 🧰 Tech Stack:-
- Java 17
- Spring Boot 3.x
- Spring Web
- Spring Data JPA
- MySQL
- Eureka Client
- OpenFeign
- Maven
 
## 📁 Project Structure:-
student-service/
laptop-service/
Each service runs independently and communicates via REST using Feign Clients.

## 🧪 Features:-

### 👨‍🎓 Student Service:-
- Add, update, delete student
- Get student by ID
- Fetch  laptop linked to a student (via Feign)

### 💻 Laptop Service:-
- Add, update, delete laptop
- Get laptops by student ID
- Each laptop is linked to one student (One-to-One)

## 🛠️ How to Run:-

### ✅ Prerequisites:-
- JDK 17
- Maven
- MySQL/ PostgreSQL running
- IntelliJ / Eclipse

 ### 🚀 Steps to Run:-
 
1. **Start PostgreSQL/MySQL** and ensure DB is created.
2. **Run Eureka Server** (if using service registry)
3. **Run Laptop Service**
4.**Run Student Service**

🌐 Sample Endpoints

👨‍🎓 Student:-

POST /student/add – Add new student

GET /student/{id} – Get student by ID

GET /student/{id}/laptops – Get  laptops for a student (via Feign)

DELETE /student/{id} – Delete student

💻 Laptop:-

POST /laptop/add – Add new laptop

GET /laptop/student/{studentId} – Get  laptops for a student

DELETE /laptop/{id} – Delete laptop

🖼️ ER Diagram 
Student (1) ——> (1) Laptop

📫 Author
Dhivya S
Junior  Developer  | Strong in Core Java,Spring Boot,Spring Security,Microservices
🔗dhivya-sekar-42b27228a

📜 License
This project is open for learning and demo purposes.












