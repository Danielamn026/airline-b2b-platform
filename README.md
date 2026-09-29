# Airline Service B2B

Plataforma moderna para operar y gestionar servicios B2B del ecosistema de aerolíneas, con una arquitectura modular que separa la experiencia de usuario del backend y la lógica de negocio.

Este repositorio reúne la aplicación frontend, la API backend y la infraestructura necesaria para ejecutar el proyecto de forma local y reproducible con Docker.

## ✨ Descripción general

La solución está pensada para representar un sistema de negocio de aerolíneas con una estructura clara y mantenible:

- Frontend en Angular para la interfaz web
- Backend en Java + Spring Boot para APIs y lógica de negocio
- Persistencia con PostgreSQL
- Ejecución local con Docker Compose
- Configuración por entorno para facilitar despliegues y pruebas

## 🧩 Características principales

- Arquitectura dividida por capas: frontend y backend
- Interfaz moderna con Angular + Tailwind CSS
- API REST construida con Spring Boot
- Validación de entrada, persistence y lógica de negocio separada
- Base de datos gestionada con PostgreSQL
- Entorno listo para correr con Docker y Docker Compose
- Estructura preparada para crecer hacia más módulos o servicios

## 🏗️ Arquitectura del proyecto

```text
airline-b2b-platform/
├── backend/                  # API REST y lógica de negocio
│   ├── src/
│   ├── .env.template
│   ├── Dockerfile
│   ├── pom.xml
│   ├── mvnw
│   └── ...
├── frontend/                 # Aplicación Angular
│   ├── src/
│   ├── package.json
│   ├── angular.json
│   ├── Dockerfile
│   └── ...
├── docker-compose.yml        # Orquestación de servicios
├── .gitignore
├── README.md
└── ...
```

### Componentes principales

- Frontend: aplicación web en Angular 21
- Backend: API REST en Spring Boot 4 con Java 17+
- Base de datos: PostgreSQL
- Infraestructura: Docker Compose para levantar el entorno

## 🛠️ Stack tecnológico

### Frontend

- Angular
- TypeScript
- Tailwind CSS
- SCSS
- Vitest

### Backend

- Java 17+
- Spring Boot
- Spring Web
- Spring Data JPA
- Spring Validation
- PostgreSQL Driver
- MapStruct
- Lombok

### Infraestructura

- Docker
- Docker Compose
- PostgreSQL

## 🚀 Inicio rápido

### Prerrequisitos

Asegúrate de tener instalado:

- Java 17 o superior
- Maven o el wrapper incluido (`./mvnw`)
- Node.js 18+
- npm
- Docker y Docker Compose

### 1. Clonar el repositorio

```bash
git clone https://github.com/Danielamn026/airline-b2b-platform.git
cd airline-b2b-platform
```

### 2. Configurar variables de entorno

Copia el archivo de ejemplo del backend:

```bash
cp backend/.env.template backend/.env
```

Ajusta los valores de conexión a la base de datos y cualquier configuración necesaria.

### 3. Ejecutar el proyecto

Con Docker Compose:

```bash
docker compose up --build
```

Esto levantará:

- Frontend: http://localhost:4200
- Backend: http://localhost:8080
- Base de datos: PostgreSQL en la red interna del contenedor

## 📁 Estructura funcional

- `frontend/`: interfaz de usuario y experiencia web
- `backend/`: servicios REST, entidades, repositorios y lógica de negocio
- `docker-compose.yml`: definición de servicios para entorno de desarrollo

## 🔐 Variables de entorno

El proyecto usa variables de entorno para la configuración de la base de datos y servicios.

Ejemplo típico:

```env
DB_URL=jdbc:postgresql://localhost:5432/airline_db
DB_USERNAME=postgres
DB_PASSWORD=your_password
```

## 🧪 Desarrollo

### Frontend

```bash
cd frontend
npm install
npm start
```

### Backend

```bash
cd backend
./mvnw clean install
./mvnw spring-boot:run
```
