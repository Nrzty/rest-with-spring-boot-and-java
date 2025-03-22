# REST API with Spring Boot - Greeting Controller

## Overview
This project is a simple REST API built with Spring Boot. It provides a single endpoint to generate personalized greeting messages.

## Features
- Exposes a REST endpoint `/greeting`.
- Accepts an optional query parameter `name` to personalize the greeting.
- Returns a JSON response containing an ID and the greeting message.

## Technologies Used
- Java
- Spring Boot
- REST API

## Installation and Setup
### Prerequisites
Ensure you have the following installed:
- Java 17 or higher
- Maven

### Clone the Repository
```sh
git clone https://github.com/Nrzty/rest-with-spring-boot-and-java/.git
cd rest-with-spring-boot-and-java
```

### Build and Run the Application
```sh
mvn spring-boot:run
```

The application will start on `http://localhost:8080`.

## API Endpoints
### Greeting Endpoint
#### Request
- **Method:** GET
- **URL:** `http://localhost:8080/greeting`
- **Query Parameters:**
  - `name` (optional): The name to be included in the greeting.

#### Example Requests
**Default Greeting:**
```sh
curl http://localhost:8080/greeting
```

#### Response Format
```json
{
  "id": 1,
  "content": "Hello, World!"
}
```


**Personalized Greeting:**
```sh
curl http://localhost:8080/greeting?name=Silvio
```

#### Response Format
```json
{
  "id": 1,
  "content": "Hello, Silvio!"
}
```

## License
This project is open-source and available under the MIT License.

## Author
Developed by NRZTY.

## Contributing
Feel free to submit issues or pull requests to improve the project.

