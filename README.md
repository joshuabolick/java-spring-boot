# Task Manager

A REST API application built with Java and Spring Boot for managing tasks.

## Features
- CRUD operations for tasks
- H2 in-memory database
- RESTful API endpoints
- JPA for data persistence

## API Endpoints
- GET `/api/tasks` - Get all tasks
- GET `/api/tasks/{id}` - Get a specific task
- POST `/api/tasks` - Create a new task
- PUT `/api/tasks/{id}` - Update an existing task
- DELETE `/api/tasks/{id}` - Delete a task

## Running the Application
1. Ensure you have Java 21 installed
2. Run `mvn spring-boot:run`
3. The application will start on port 8080
4. Access the H2 console at `http://localhost:8080/h2-console`

## Example API Usage
```bash
# Create a new task
curl -X POST http://localhost:8080/api/tasks \
-H "Content-Type: application/json" \
-d '{
    "title": "Complete project",
    "description": "Finish the Spring Boot project",
    "completed": false
}'
```
