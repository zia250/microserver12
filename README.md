# Node.js Microservices Project

This repository contains a Node.js-based microservices architecture project. Each microservice is designed to handle a specific domain within the system.

## Project Structure


nodejs_microservice_master/
|-- customer/        # Customer microservice
|-- db/              # Database configurations
|-- gateway/         # API Gateway
|-- products/        # Products microservice
|-- proxy/           # Proxy service
|-- shopping/        # Shopping microservice
|-- docker-compose.yml # Docker Compose file for containerization
|-- README.md         # Project documentation


### Microservices

1. *Customer Service*
   - Manages customer-related operations.

2. *Products Service*
   - Handles product catalog and related actions.

3. *Shopping Service*
   - Manages shopping cart and orders.

4. *Gateway*
   - Serves as the API Gateway for routing requests to appropriate services.

5. *Proxy*
   - Implements proxy functionality for added abstraction or performance enhancements.

### Database

- The db folder contains configurations for setting up and managing the database used by the microservices.

### Docker Compose

- The docker-compose.yml file defines the containerized services and their interconnections for easy deployment.

## Prerequisites

- [Node.js](https://nodejs.org/) (v14 or above)
- [Docker](https://www.docker.com/) (for containerization)
- [npm](https://www.npmjs.com/) (Node package manager)

## Setup and Usage

1. Clone the repository:
   bash
   git clone <repository-url>
   cd nodejs_microservice_master
   

2. Install dependencies for each microservice:
   bash
   cd customer
   npm install
   cd ../products
   npm install
   # Repeat for other services
   

3. Start the services using Docker Compose:
   bash
   docker-compose up --build
   

4. Access the API Gateway (default port: 8080):
   
   http://localhost:8080
   

## Contribution

1. Fork the repository.
2. Create a new branch for your feature/bugfix.
3. Submit a pull request.

