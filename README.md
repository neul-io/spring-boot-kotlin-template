# Spring Boot Kotlin Template

A minimal Spring Boot web application template using Kotlin.

## Getting Started

### Prerequisites

- Java 21 or later
- Gradle 8.x or later (or use the included Gradle wrapper)

### Running Locally

```bash
# Run with Gradle wrapper
./gradlew bootRun
```

The server will start on port 8080 (or the port specified in the `PORT` environment variable).

### Endpoints

- `GET /` - Hello World response
- `GET /actuator/health` - Health check endpoint

### Building for Production

```bash
./gradlew bootJar
java -jar build/libs/*.jar
```

## Project Structure

```
.
├── src/main/kotlin/com/example/app/
│   ├── Application.kt       # Application entry point
│   └── HelloController.kt   # REST controller
├── src/main/resources/
│   └── application.properties  # Configuration
├── build.gradle.kts         # Gradle dependencies
└── README.md                # This file
```

## License

MIT
