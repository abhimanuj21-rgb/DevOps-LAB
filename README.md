# Task Manager

A simple Java Spring Boot application for managing tasks locally with CRUD functionality.

## Features
- Create tasks
- View all tasks
- Update task status, priority, and description
- Delete tasks
- Local H2 in-memory database
- Simple web interface

## Run locally

1. Make sure Java 17+ is installed.
2. From the project root, run:

```bash
mvn spring-boot:run
```

3. Open the app in your browser:

```text
http://localhost:8080
```

4. H2 database console:

```text
http://localhost:8080/h2-console
```

Use these database connection settings:
- JDBC URL: `jdbc:h2:mem:taskdb`
- Username: `sa`
- Password: empty

## Project structure
- `src/main/java/com/taskmanager/taskmanager` - Java application code
- `src/main/resources/static` - Web UI
- `src/main/resources/application.properties` - Spring Boot configuration

## Notes
This project stores data in an in-memory H2 database, so tasks are reset when the server restarts.
