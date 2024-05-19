# ChatApp

A real-time chat application built with Spring Boot that allows users to connect, send messages, and interact in a chat room.

## Prerequisites

- Java 11 or above
- Maven

## Installation

1. Clone the repository.
   ```bash
   git clone https://github.com/rajneeshkabdwal4/chat
   ```
2. Navigate to the project directory.
   ```bash
   cd chat
   ```
3. Install the dependencies.
   ```bash
   ./mvnw install
   ```

## Running the Application

To start the application, run:
```bash
./mvnw spring-boot:run
```

## Project Structure

The project is structured as follows:

### `src/main/java`

Contains the Java source code for the application.

- **com.example.chat**: Replace with your base package name.
  - **chat**: Contains the core application classes for chat functionality.
    - `ChatMessage.java`: Represents a chat message object.
    - `MessageType.java` (Optional): Defines the message types used in the application (e.g., JOIN, LEAVE, MESSAGE).
    - `ChatController.java`: Handles incoming and outgoing chat messages.
  - **config**: Contains configuration classes for the application.
    - `WebSocketConfig.java`: Configures the WebSocket endpoint and message broker (if using a message broker).
  - `ChatApplication.java`: The main Spring Boot application class.

### `src/main/resources`

Contains application resources.

- **static**: Contains static resources such as CSS and JavaScript files for your chat interface.
- **templates**: Contains HTML templates used by the application.
  - `index.html`: The main chat application template. (Replace with relevant template name if different)
- `application.properties`: Contains configuration properties for the application, including WebSocket endpoint URL and (potentially) message broker details.

### `src/test/java`

Contains unit and integration tests for the application (if applicable).

### `.gitignore`

Specifies files and directories to be ignored by Git.

### `README.md`

This readme file.

### `mvnw`

Maven wrapper script for running Maven commands.

### `mvnw.cmd`

Windows batch script for running Maven commands (Windows only).

### `pom.xml`

The project object model (POM) file that defines the project dependencies and build configuration. Configure this as needed for your project.
