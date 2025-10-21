# Yushan Config Server

Centralized configuration management server for Yushan Novel Platform microservices.

## Features

- Centralized configuration management
- Git-backed configuration storage
- Service discovery via Eureka
- Environment-specific configurations
- Automatic configuration refresh

## Running Locally

### Prerequisites
- Java 21+
- Maven 3.8+
- Eureka Server running on port 8761
- Git repository with configuration files (or use native profile)

### Start with Native Profile (Local Testing)
```bash
./mvnw spring-boot:run -Dspring-boot.run.profiles=native
```

### Start with Git Profile (Production)
```bash
./mvnw spring-boot:run
```

The config server will start on port 8888.

## Configuration Structure

### Git Repository Structure