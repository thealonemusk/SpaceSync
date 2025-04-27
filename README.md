# SpaceSync

SpaceSync is a real-time space occupancy management platform designed to optimize the use of office spaces. It tracks desk and room usage within corporate buildings and provides live occupancy data, updating in real-time via WebSocket.

## Tech Stack

- **Frontend:** React.js
- **Backend:** Java (Vert.x microservices)
- **Real-time:** WebSocket
- **Database:** PostgreSQL
- **Cache:** Redis
- **Containerization:** Docker
- **Cloud/Orchestration:** AWS EKS (Elastic Kubernetes Service)

## Project Structure

```
SpaceSync/
├── frontend/           # React.js frontend application
├── backend/            # Java backend using Vert.x
│   ├── src/            # Source code
│   ├── tests/          # Unit and integration tests
│   └── pom.xml         # Maven configuration
├── docker/             # Dockerfiles and docker-compose files
├── kubernetes/         # Kubernetes manifests for deployment on AWS EKS
├── docs/               # Documentation
└── README.md           # Project overview and setup instructions
```

## Setup Instructions

### Prerequisites

- Node.js and npm (for frontend)
- Java JDK 11 or later (for backend)
- Docker and Docker Compose
- AWS CLI configured (for EKS deployment)
- PostgreSQL and Redis (or use Docker containers)

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Build the project using Maven:
   ```bash
   mvn clean install
   ```
3. Run the application:
   ```bash
   mvn vertx:run
   ```

### Docker Setup

1. Navigate to the docker directory:
   ```bash
   cd docker
   ```
2. Build and start the containers:
   ```bash
   docker-compose up -d
   ```

### Kubernetes Deployment

1. Navigate to the kubernetes directory:
   ```bash
   cd kubernetes
   ```
2. Apply the Kubernetes manifests:
   ```bash
   kubectl apply -f .
   ```

## License

This project is licensed under the MIT License.
