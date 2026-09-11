# SmartFlow

SmartFlow is an AI-powered smart task management application designed to help users organize tasks, manage priorities, build productive habits, and work more efficiently.

The application focuses on modern Java development, clean architecture, and practical AI integration.

---

## 🎯 Project Goals

The main goals of this project are:

* Build a production-style application using modern Java and Spring Boot.
* Apply clean architecture and maintainable code structure.
* Integrate AI features into a practical task management application.
* Demonstrate real-world backend development skills.
* Create a project that can be presented to potential employers.

---

## 🛠️ Current Technologies

* Java 21
* Spring Boot
* Maven
* REST API
* Git
* GitHub

### Technologies Planned for the Project

* PostgreSQL
* Spring Data JPA
* Flyway
* Testcontainers
* Docker
* AI API integration
* Spring Security
* JWT Authentication
* OpenAPI / Swagger
* CI/CD

---

## ✨ Planned Features

### Task Management

* Create, update, and delete tasks.
* Set task priorities:

    * LOW
    * MEDIUM
    * HIGH
* Manage task statuses:

    * TODO
    * IN_PROGRESS
    * COMPLETED
* Add optional task descriptions.
* Categorize tasks.
* Add reminders.
* Create recurring tasks.

### Category Management

* Users can create, update, and delete their own categories.
* Category names are unique per user.
* Category name uniqueness is case-insensitive.
* Tasks can optionally belong to a category.

### AI Features

Planned AI capabilities include:

* AI-generated task suggestions.
* Automatic task prioritization.
* Natural language task creation.
* Task breakdown into smaller steps.
* Productivity insights and recommendations.

### Future Features

* User authentication and authorization.
* Notifications and reminders.
* Task search and filtering.
* Dashboard and productivity statistics.
* Dockerized application.
* Automated tests.
* CI/CD pipeline.

---

## 🏗️ Architecture Overview

The project follows a feature-based package structure to keep the code organized and scalable as the application grows.

Example:

```text
com.smartflow
│
├── health
│   └── api
│
├── category
│   ├── api
│   ├── application
│   └── domain
│
├── task
│   ├── api
│   ├── application
│   └── domain
│
└── user
    ├── api
    ├── application
    └── domain
```

Each feature is responsible for its own functionality and keeps related code close together.

The architecture will continue to evolve as new features and technologies are introduced.

---

## 🚧 Current Project Status

### Completed

* [x] Initialize Spring Boot project.
* [x] Configure Java 21.
* [x] Create SmartFlow application entry point.
* [x] Create and test a Health API endpoint.
* [x] Set up local Git repository.
* [x] Connect project to GitHub.

### Currently Working On

* [ ] Define the domain model.
* [ ] Implement Category Management.

---

## 🚀 Getting Started

### Prerequisites

* Java 21

### Run the Application

Clone the repository:

```bash
git clone https://github.com/KenanSpahic/ai-smart-task-manager.git
```

Navigate to the project directory:

```bash
cd ai-smart-task-manager
```

Run the application using Maven Wrapper.

**Windows:**

```bash
mvnw.cmd spring-boot:run
```

**macOS/Linux:**

```bash
./mvnw spring-boot:run
```

The application starts on:

```text
http://localhost:8080
```

### Health Check

```text
GET http://localhost:8080/api/v1/health
```

Example response:

```json
{
  "status": "UP"
}
```
