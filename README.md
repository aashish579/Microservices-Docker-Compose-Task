# Microservices Containerization Assessment

## Skill Test 1: Cloud and Containers

Submitted by: Aashish Gautam

GitHub Repository:
https://github.com/aashish579/Microservices-Docker-Compose-Task

## Project Overview

This project demonstrates containerization of four Node.js
microservices using Docker and Docker Compose.

## Microservices

| Service | Port | Endpoint |
|---|---|---|
| User Service | 3000 | /users |
| Product Service | 3001 | /products |
| Order Service | 3002 | /orders |
| Gateway Service | 3003 | /health |

## Technologies

- Node.js
- Express.js
- Docker
- Docker Compose
- Docker Bridge Network
- REST APIs

## Setup Instructions

1. Install Docker Desktop and Git.
2. Clone the repository.
3. Navigate to the project directory.
4. Execute: docker compose up --build -d
5. Verify: docker compose ps

## API Testing

User Service:
http://localhost:3000/users

Product Service:
http://localhost:3001/products

Order Service:
http://localhost:3002/orders

Gateway Health:
http://localhost:3003/health

Gateway User API:
http://localhost:3003/api/users

Gateway Product API:
http://localhost:3003/api/products

Gateway Order API:
http://localhost:3003/api/orders

## Test Results

All four Docker containers started successfully.

All seven endpoints returned HTTP 200.

The Gateway Service successfully communicates with the
User, Product and Order services through the Docker network.

## Troubleshooting

Docker not running:
Start Docker Desktop and verify using docker info.

Port conflict:
Stop the process occupying ports 3000-3003.

Container startup failure:
Run docker compose logs.

Build failure:
Run docker compose up --build -d.

## Evidence

Screenshots are available in the screenshots folder.

## Stop Containers

docker compose down
