# ToDoApp
This is a simple Todo App built using Spring Boot, MySQL, JPA, and JSP. It allows users to manage their todo items efficiently with functionalities to add, edit, delete, mark as complete/incomplete, and view all items.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Approach](#approach)
- [Challenges Faced](#challenges-faced)


## Features
1. Add Todo Item: User can add a new todo item.
2. Edit Todo Item: User can edit an existing todo item.
3. Delete Todo Item: User can delete a todo item.
4. Mark as Complete/Incomplete: User can mark a todo item as complete or incomplete.
5. View Todo Items: User can view a list of all todo items.

## Installation
### Prerequisites
- Java 11 or higher
- Maven
- MySQL

### Steps
1. Clone the repository:
   
    git clone https://github.com/mandarmaske01/ToDoApp.git

    
2. Navigate to the project directory:
   
    cd ToDoApp
    
3. Configure the database:
   - Create a MySQL database named todo_db.
   - Update the application.properties file with your MySQL username and password.
    
     spring.datasource.url=jdbc:mysql://localhost:3306/todo_db
     spring.datasource.username=root
     spring.datasource.password=root
     spring.jpa.hibernate.ddl-auto=update
     
4. Build the project:
   
    mvn clean install
    
5. Run the application:
   
    mvn spring-boot:run
    
## Usage
1. Use the interface to add, edit, delete, and manage your todo items.

## Approach
### Backend
- The backend is developed using Spring Boot to handle the business logic.
- JPA (Java Persistence API) is used for data access and manipulation.
- MySQL is used as the database to store todo items.

### Frontend
- The frontend is developed using JSP to provide a dynamic web interface.
- The user can perform CRUD operations (Create, Read, Update, Delete) on todo items through the web interface.

## Challenges Faced
1. Database Connectivity: Initial setup and configuration of the MySQL database to work seamlessly with Spring Boot.
2. JPA Mappings: Ensuring correct JPA mappings for the Todo entity to handle CRUD operations efficiently.
3. UI Design: Creating a user-friendly interface using JSP and ensuring that the frontend communicates properly with the backend.
4. Error Handling: Implementing robust error handling to manage potential issues such as database connection failures or invalid user inputs.

Despite these challenges, the core functionalities of the Todo App were successfully implemented.

