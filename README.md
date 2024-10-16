# Simple REST Service

This project is a basic RESTful web service built using Spring Boot. It provides a simple API that returns a greeting message.

## Features
- Basic RESTful endpoint to return a greeting message.
- Supports a query parameter to customize the greeting message.

## Tools and Technologies
- Java 11 (or higher)
- Spring Boot 2.7.0 (or the version used in your project)
- Maven
- Postman (or any REST client for testing)

## How to Run the Application

### 1. Using IntelliJ IDEA (or any other IDE)
1. Import the project into IntelliJ.
2. Navigate to the `SimpleRestServiceApplication.java` file in `src/main/java/com/example/simple_rest_service`.
3. Right-click the file and choose **Run 'SimpleRestServiceApplication'** to start the server.

### 2. Using Maven (Command Line)
1. Open a terminal and navigate to the project directory.
2. Run the following Maven command to start the application:
   ```bash
   mvn spring-boot:run
3. The application will start on the default port 8080.

## How to Test the API
You can test the API using Postman or any REST client. The following endpoints are available:

1. Default Greeting
   - Request: GET http://localhost:8080/greeting
   - Response:
    ```json
   {
   "id": 1,
   "content": "Hello, World!"
   }
2. Custom Greeting
   - Request: GET http://localhost:8080/greeting?name=Kalyani
   - Response:
    ```json
   {
   "id": 2,
   "content": "Hello, Kalyani!"
   }

## Project Structure

```json 
    simple_rest_services/
    ├── src/
    │   ├── main/
    │   │   ├── java/
    │   │   │   └── com/
    │   │   │       └── example/
    │   │   │           └── simple_rest_service/
    │   │   │               ├── controller/
    │   │   │               │   └── GreetingController.java
    │   │   │               ├── model/
    │   │   │               │   └── Greeting.java
    │   │   │               └── SimpleRestServiceApplication.java
    │   └── resources/
    ├── pom.xml
    └── README.md
