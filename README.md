# EshopMicroservices

A microservices-based architecture designed for an e-commerce application using domain-driven design (DDD), clean architecture, and modern design patterns. This project integrates several libraries and frameworks to ensure scalability, performance, and maintainability.

## Architecture Overview

The project follows the **Layered Architecture** with a combination of:
- **DDD (Domain-Driven Design)**: Organizing code around business concepts for better maintainability and understanding.
- **Vertical Slice Architecture**: Splitting the codebase into feature-specific slices to reduce complexity.
- **Clean Architecture**: Ensuring a clear separation of concerns, making the system flexible and easy to modify.

## Design Patterns Used
- **SOLID**: Adherence to the five principles of object-oriented design for more scalable and maintainable code.
- **CQRS (Command Query Responsibility Segregation)**: Separating read and write operations to optimize performance and scalability.
- **Mediator**: Centralizing communication between components to reduce dependencies.
- **Decorator**: Extending functionality of objects in a flexible and reusable manner.
- **Pub/Sub (Publish/Subscribe)**: Asynchronous communication pattern for decoupling components.
- **Caching**: Implementing caching mechanisms to optimize data retrieval and reduce database load.
- **API Gateway**: Managing all API traffic and routing to the appropriate microservices.

## Tech Stack

### Databases:
- **Postgres**: Relational database for storing transactional data.
- **Redis**: In-memory data store for caching and session management.
- **SQLite**: Lightweight database for local storage or development environments.
- **SQL Server**: Another relational database option for enterprise environments.

### Libraries and Tools:
- **Carter**: Minimal API framework for building REST APIs quickly.
- **Marten**: Provides transactional document storage on top of PostgreSQL.
- **MediatR**: Helps in implementing the mediator pattern for decoupled communication between services.
- **Mapster**: Object mapping library for transforming data models.
- **MassTransit**: Distributed application framework for building asynchronous communication with message brokers.
- **FluentValidation**: Provides a fluent interface for defining validation rules.
- **EFCore (Entity Framework Core)**: Object-relational mapper for working with databases in .NET.
- **Refit**: REST library for making HTTP requests in a clean and type-safe way.

### Communication Protocols:
- **gRPC**: High-performance, synchronous communication between microservices.
- **YARP (Yet Another Reverse Proxy)**: API gateway to route requests to different services.

## Features
- **Scalability**: The microservices architecture allows easy scaling by adding or removing services.
- **Modularity**: With a clear separation of concerns, each service is independently deployable.
- **Asynchronous Communication**: Using Pub/Sub, MassTransit, and gRPC to enable efficient, real-time data flow.
- **Caching**: Redis is used for caching frequently accessed data, ensuring faster responses and reduced load on databases.

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/EshopMicroservices.git
