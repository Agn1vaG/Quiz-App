# Quiz-App

A simple **Spring Boot** project that provides an API to fetch random programming-related questions from a selected category. It uses **PostgreSQL** as the database and allows users to retrieve quiz questions based on their preferred programming language.

## Features
- Fetch random questions from a specified programming category
- Built using **Spring Boot** for backend development
- Uses **PostgreSQL** as the database
- Provides a **RESTful API** for easy integration

## Technologies Used
- **Spring Boot** (Backend Framework)
- **PostgreSQL** (Database)
- **JPA/Hibernate** (ORM for database interaction)

## How It Works
1. The API allows users to request questions from a specific programming category.
2. It retrieves a set number of random questions from the database.
3. The questions are returned as **JSON responses** for frontend or application integration.

## Setup Instructions

### Clone the repository:
```sh
git clone https://github.com/your-username/Quiz-App.git  
cd Quiz-App  
```

### Configure the database in `application.properties`:
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/quizdb  
spring.datasource.username=your-username  
spring.datasource.password=your-password  
```

### Run the application using:
```sh
mvn spring-boot:run  
```

### Access the API via:
```sh
GET http://localhost:8080/quiz?category=Java&numQ=5  
```

## Future Enhancements
- Add **user authentication**
- Support **multiple-choice answers**
- Implement a **frontend UI**

