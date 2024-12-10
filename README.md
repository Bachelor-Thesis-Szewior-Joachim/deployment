# Project Overview

This project consists of a **Frontend** and a **Backend**, both of which are Dockerized for easy setup and deployment. The backend uses Java with Maven, while the frontend is built with React and Node.js. This project also includes Docker Compose for managing both services together.

## Backend

The backend is a Java Spring Boot application. It is responsible for handling API requests and connecting to the database, solana server and model server. The backend uses Maven for dependency management and build automation.

## Frontend

The frontend is a React-based application that communicates with the backend via API calls. The application is Dockerized for easier deployment.

### Setup

1. **Clone the repository**:
   ```bash
   git clone --recurse-submodules https://github.com/Bachelor-Thesis-Szewior-Joachim/deployment.git
   ```

## Docker Compose

The `docker-compose.yml` file manages the services for all containers(backend, frontend, database, solana and model).

### Running the Project with Docker Compose

To start both the frontend and backend services along with the database, run the following command:

```bash
docker compose up
```

This will pull the necessary images and start the containers for the frontend, backend, solana, model and database. The services will be accessible as follows:

- **Frontend**: `http://localhost:3000`
- **Backend**: `http://localhost:8080`

### Stopping the Services

To stop the services, run:

```bash
docker compose down
```

## Conclusion

This project is a full-stack application with a Dockerized all services. 