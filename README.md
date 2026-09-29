# Airline Service B2B

A modern B2B airline service platform built with a modular architecture that separates the user-facing frontend from the backend business services. The project is designed to support airline operations, service orchestration, and business workflows in a clean and scalable way.

## Overview

This repository contains the complete source code for the Airline Service B2B platform, including:

- Angular frontend for the web application
- Java Spring Boot backend for APIs and business logic
- PostgreSQL database integration
- Docker-based runtime setup for local development and deployment
- Environment configuration files for service isolation and setup consistency

The project is structured to support clear separation of concerns and easier maintainability as the platform grows.

## Architecture

The solution is organized in two main layers:

- Frontend: Angular application with modern UI practices and Tailwind styling
- Backend: Spring Boot application with REST APIs, persistence layer, validation, and service logic

### Runtime Components

- Frontend application running on port 4200
- Backend API running on port 8080
- PostgreSQL database configured through environment variables
- Docker Compose orchestrates the application services

## Repository Structure

```text
airline-service-b2b/
├── backend/
│   ├── .env.template
│   ├── .mvn/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   └── resources/
│   │   └── test/
│   ├── Dockerfile
│   ├── pom.xml
│   ├── mvnw
│   ├── mvnw.cmd
│   └── http-tests/
├── frontend/
│   ├── src/
│   ├── public/
│   ├── Dockerfile
│   ├── angular.json
│   ├── package.json
│   ├── tsconfig.json
│   ├── README.md
│   └── ...
├── docker-compose.yml
├── .gitignore
└── README.md
```
## Tech Stack

### Frontend

| Technology | Version | Purpose |
|---|---|---|
| Angular | 21.2.0 | Framework |
| TypeScript | 5.9.2 | Language |
| Tailwind CSS | 4.2.2 | Styling |
| SCSS | Latest | Advanced styling |
| Vite/Vitest | 4.0.8 | Testing |
| PostCSS | 8.5.8 | CSS Processing |
| Prettier | 3.8.1 | Code formatting |

### Backend

| Technology | Version | Purpose |
|---|---|---|
| Java | 17+ | Language |
| Spring Boot | 4.0.5 | Framework |
| Spring Web | Latest | REST APIs |
| Spring Data JPA | Latest | Persistence |
| PostgreSQL Driver | Latest | Database driver |
| Spring Validation | Latest | Input validation |
| MapStruct | 1.6.3 | Object mapping |
| Lombok | Latest | Code generation |

### Infrastructure

| Technology | Version | Purpose |
|---|---|---|
| Docker | Latest | Containerization |
| Docker Compose | Latest | Orchestration |
| NGINX | Latest | Frontend serving |
| PostgreSQL | 12+ | Database |

## Prerequisites

Before running the project, ensure you have the following installed:

- **Java 17** or newer
- **Maven** (or use the included Maven wrapper: `./mvnw`)
- **Node.js** 18 or newer
- **npm** 10.9.2 or newer
- **Docker** and **Docker Compose** (for containerized setup)
- **PostgreSQL** 12 or newer (if running without Docker)

