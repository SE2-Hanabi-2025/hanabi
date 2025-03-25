# Hanabi Server

This is the backend server for the **Hanabi** multiplayer game, built using **Spring Boot**.

## Requirements

- **Java 17+** (or a compatible version)
- **Gradle** (for building and running the project)
- **Maven** (optional, if you use it instead of Gradle)

## Getting Started

1. **Clone the repository**:
   git clone https://github.com/SE2-Hanabi-2025/hanabi

2. **Make sure you are in the server subdirectory**
    cd server

3. **Build the server using Gradle**
    ./gradlew build

4. **Run the server**
    ./gradlew bootRun


## Endpoints

Here are the basic endpoints available on the server:

- **`/connect`** (POST)
  - **Description**: Connects a player to the game.
  - **Response**: `200 OK` or error message if the connection fails.

- **`/start-game`** (POST)
  - **Description**: Starts a new game.
  - **Response**: `200 OK` with game status, or error message if game cannot start.

- **`/status`** (GET)
  - **Description**: Checks the current status of the game (e.g., if the game is in progress).
  - **Response**: JSON response with the game status.

## Additional Information

- The server uses **Spring Boot** for quick setup and REST API endpoints.
- The server listens on **`localhost:8080`** by default, and you can modify this in the `application.properties` file.
