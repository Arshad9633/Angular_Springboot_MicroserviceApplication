# Angular-Springboot Microservices Application

## Overview

This project is a comprehensive **microservices-based application** built using **Spring Boot** for the backend and **Angular v18** for the frontend. The application is divided into multiple services, each serving a specific functionality such as **ProductService**, **OrderService**, **InventoryService**, and an **API Gateway** for routing.

We use **Spring Cloud OpenFeign** for synchronous communication between services, **Resilience4J** for circuit breaker implementation, and **Keycloak** for securing the API Gateway. The UI is developed using the latest version of Angular.

## Microservices Architecture

The application is broken down into the following services:
1. **ProductService**: Manages product-related operations.
2. **OrderService**: Manages customer orders and communicates with InventoryService.
3. **InventoryService**: Manages the inventory of products.
4. **API Gateway**: Routes and secures the microservices using Keycloak.

### Key Technologies Used:
- **Spring Boot**: Backend framework for microservices.
- **Angular v18**: Frontend framework for building the user interface.
- **Spring Cloud OpenFeign**: For synchronous communication between services.
- **Resilience4J**: For implementing the Circuit Breaker pattern.
- **Keycloak**: For API Gateway security.
- **Spring Cloud Circuit Breaker**: Used in conjunction with Resilience4J for circuit breaker functionality.

---

## Features

- **Synchronous Communication**: The OrderService communicates with the InventoryService using the Spring Cloud OpenFeign library.
- **Declarative REST Client**: OpenFeign simplifies RESTful API consumption with minimal configuration.
- **Circuit Breaker**: Implemented using Resilience4J to ensure resiliency and fault tolerance in the application.
- **API Security**: The API Gateway is secured using Keycloak for authentication and authorization.
- **Responsive UI**: The user interface is built with Angular v18, providing an intuitive and seamless experience.

---

## Installation & Setup

### Prerequisites

- **Java 17+** installed on your machine.
- **Node.js** (for Angular frontend) installed on your machine.
- **Angular CLI** installed globally:
  ```bash
  npm install -g @angular/cli
