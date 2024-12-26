# Banking Application

## Overview

This project is a simple banking application built using Spring Boot. 
It provides RESTful APIs for managing bank accounts, including operations 
such as creating accounts, depositing money, withdrawing money, 
retrieving account details, and deleting accounts.

## GitHub Repository:
https://github.com/Sesa-ja/OOP-Final-Project-Baking-App.git
## Render link (Deployment)
https://oop-final-project-baking-app.onrender.com

## **REST API Documentation**
The REST APIs are documented using Swagger. You can access the Swagger UI to explore 
and test the APIs.

## API Endpoints

### 1. Create an Account
URL: /api/accounts
Method: POST
Request Body:

{
"id": null,
"accountHolderName": "John Doe",
"balance": 1000.0
}

Response:
{
"id": 1,
"accountHolderName": "John Doe",
"balance": 1000.0
}

### 2. Get an Account by ID
URL: /api/accounts/{id}
Method: GET
Response:

{
"id": 1,
"accountHolderName": "John Doe",
"balance": 1000.0
}

### 3. Deposit Money
URL: /api/accounts/{id}/deposit
Method: PUT
Request Body:

{
"amount": 500.0
}

Response:

{
"id": 1,
"accountHolderName": "John Doe",
"balance": 1500.0
}

### 4. Withdraw Money
URL: /api/accounts/{id}/withdraw
Method: PUT
Request Body:

{
"amount": 300.0
}

Response:

{
"id": 1,
"accountHolderName": "John Doe",
"balance": 1200.0
}

### 5. Get All Accounts
URL: /api/accounts
Method: GET
Response:

[
{
"id": 1,
"accountHolderName": "John Doe",
"balance": 1200.0
},
{
"id": 2,
"accountHolderName": "Jane Smith",
"balance": 2000.0
}
]

### 6. Delete an Account
URL: /api/accounts/{id}
Method: DELETE
Response:

"Account deleted"

## Technological Stack

### Backend
Language: Java
Framework: Spring Boot
Libraries:
Spring Web
Spring Data JPA
MySql Database
Lombok

#### Database

Type: MySQl
Tool: Sql
Console URL: http://localhost:8080/MySql-console

#### Build Tool
Maven

## How to Run the Project

### Prerequisites
Java 17 or higher
Maven

### Steps
Clone the repository: git clone <repository-url>
Navigate to the project directory: cd banking-app
Build the project: mvn clean install
Run the application: mvn spring-boot:run

## Future Enhancements
Add authentication and authorization using Spring Security.
Enable external database support (e.g., MySQL, PostgreSQL).
Implement additional banking operations, such as transfers and statements.


