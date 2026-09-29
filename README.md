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
