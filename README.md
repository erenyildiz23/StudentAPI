# StudentAPI with React.js Client

This project is a full-stack web application that combines a Spring Boot backend with a React.js frontend. The application allows for managing student information, including creating, reading, updating, and deleting student records. 

## Table of Contents
- [Technologies Used](#technologies-used)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Technologies Used

- **Backend:**
  - Java
  - Spring Boot
  - Spring Data JPA
  - PostgreSQL

- **Frontend:**
  - React.js
  - Axios (for HTTP requests)

- **Others:**
  - Lombok
  - Maven

## Prerequisites

Make sure you have the following installed on your system:

- Java 17 or higher
- Node.js and npm
- PostgreSQL
- Maven

## Installation

### Backend

1. **Clone the repository:**
    ```sh
    git clone https://github.com/erenyildiz23/StudentAPI.git
    cd StudentAPI/studentapi
    ```

2. **Set up PostgreSQL:**
    Create a database named `studentdb` and a user with the necessary permissions. Update the `application.properties` file with your database credentials.

    ```properties
    spring.datasource.url=jdbc:postgresql://localhost:5432/studentdb
    spring.datasource.username=yourusername
    spring.datasource.password=yourpassword
    spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
    spring.jpa.hibernate.ddl-auto=update
    ```

3. **Build the project:**
    ```sh
    ./mvnw clean install
    ```

### Frontend

1. **Navigate to the frontend directory:**
    ```sh
    cd ../student-api-client
    ```

2. **Install dependencies:**
    ```sh
    npm install
    ```

## Running the Application

### Backend

To run the Spring Boot application, navigate to the `studentapi` directory and use the following command:

```sh
./mvnw spring-boot:run
