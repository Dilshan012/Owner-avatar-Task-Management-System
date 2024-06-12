# Task Manager Application

## Project Description
This project is a full-stack web application that allows users to register, log in, and manage a list of tasks. The application uses Spring Boot for the back end and React.js for the front end. Authentication is implemented using JSON Web Tokens (JWT).

## Technologies Used
- **Back-End:**
  - Spring Boot
  - Spring Security
  - Spring Data JPA
  - JWT
  - MySQL (or H2 Database)
- **Front-End:**
  - React.js
  - Axios
  - Redux (or Context API)
  - Material-UI (optional)

## Features
- User registration and login
- Password hashing and secure storage
- JWT-based authentication
- CRUD operations on tasks
- Responsive UI

## Installation and Setup

### Prerequisites
- Java 11 or higher
- Node.js and npm
- MySQL (if not using H2 database)

### Back-End Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/Dilshan012/Task-Management-System.git
   cd task-manager-app

   Navigate to the back-end directory:

cd backend
Configure the database in src/main/resources/application.properties:

properties

# For H2 Database
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=password
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.h2.console.enabled=true

### For MySQL Database (Uncomment if using MySQL)
### spring.datasource.url=jdbc:mysql://localhost:3306/taskdb
### spring.datasource.username=root
### spring.datasource.password=yourpassword
### spring.jpa.hibernate.ddl-auto=update
### spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL5Dialect

- Run the Spring Boot application:
./mvnw spring-boot:run

## Front-End Setup

- Navigate to the front-end directory:
cd ../frontend

- Install dependencies:
npm install

- Run the React application:
npm start

## Running the Application
- Open your browser and navigate to http://localhost:3000.
- Register a new user and log in.
- Manage your tasks by adding, editing, and deleting them.
